## V2Ray-VPN搭建



### 安装



##### 1.安装wget

默认没有安装wget，我们需要自己安装，执行如下命令进行安装：

```
yum -y install wget
```



##### 2.下载脚本

安装完wget之后就可以进行下载操作了，如下：

```
wget https://install.direct/go.sh
```



##### 3.安装unzip

因为centos不支持apt-get，我们需要安装unzip，详见官方说明：

```
yum install -y zip unzip 
```



##### 4.执行安装



```
[michael@centos74 v2ray]$ bash go.sh 
```



##### 安装简介：

```
Installing V2Ray v3.14 on x86_64

Downloading V2Ray.

 % Total  % Received % Xferd Average Speed  Time  Time   Time Current

​                 Dload Upload  Total  Spent  Left Speed

100  608  0  608  0   0  2229   0 --:--:-- --:--:-- --:--:-- 2235

100 8482k 100 8482k  0   0 2501k   0 0:00:03 0:00:03 --:--:-- 2813k

Extracting V2Ray package to /tmp/v2ray.

Archive: /tmp/v2ray/v2ray.zip

  creating: /tmp/v2ray/v2ray-v3.14-linux-64/

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/geoip.dat 

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/geosite.dat 

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/readme.md 

  creating: /tmp/v2ray/v2ray-v3.14-linux-64/systemd/

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/systemd/v2ray.service 

  creating: /tmp/v2ray/v2ray-v3.14-linux-64/systemv/

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/systemv/v2ray 

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/v2ctl 

 extracting: /tmp/v2ray/v2ray-v3.14-linux-64/v2ctl.sig 

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/v2ray 

 extracting: /tmp/v2ray/v2ray-v3.14-linux-64/v2ray.sig 

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/vpoint_socks_vmess.json 

 inflating: /tmp/v2ray/v2ray-v3.14-linux-64/vpoint_vmess_freedom.json 

PORT:13437

UUID:f500ecf5-e135-49c6-9ce2-78eb490d0aa9

Created symlink from /etc/systemd/system/multi-user.target.wants/v2ray.service to /etc/systemd/system/v2ray.service.

V2Ray v3.14 is installed.
```



##### 5.相关命令

在首次安装完成之后，V2Ray不会自动启动，需要手动运行上述启动命令。而在已经运行V2Ray的VPS上再次执行安装脚本，安装脚本会自动停止V2Ray 进程，升级V2Ray程序，然后自动运行V2Ray。在升级过程中，配置文件不会被修改。

```
## 启动

systemctl start v2ray


\## 停止

systemctl stop v2ray


\## 重启

systemctl restart v2ray


\## 开机自启

systemctl enable v2ray
```

###### 关于软件更新：更新 V2Ray 的方法是再次执行安装脚本！再次执行安装脚本！再次执行安装脚本！



##### 6.配置v2ray服务端

假设你的域名是v2ray.com，并将二级域名hi.v2ray.com解析到你的VPS。

执行下面的命令，开始配置v2ray:

```
[root@ss-us ~]# vi /etc/v2ray/config.json 
```



按i键编辑文件，把内容更改为下面的内容：



```
{

 "log": {

  "access": "/var/log/v2ray/access.log",

  "error": "/var/log/v2ray/error.log",

  "loglevel": "warning"

 },

 "inbounds": [

  {

   "port": 33684,

   "listen": "127.0.0.1",

   "protocol": "vmess",

   "settings": {

    "clients": [

     {

      "id": "0c67ca68-63ad-40c5-898e-9cf1925c8694",

      "level": 1,

      "alterId": 64

     }

    ]

   },

   "streamSettings": {

    "network": "ws",

    "wsSettings": {

     "path": "/etc/nginx/html"//这个地址就是使用一键安装工具生成之后访问到的地址，也就是虚拟目录访问地址

    }

   }

  }

 ],

 "outbounds": [

  {

   "protocol": "freedom",

   "settings": {},

   "tag": "direct"

  },

  {

   "protocol": "blackhole",

   "settings": {},

   "tag": "blocked"

  }

 ],

 "routing": {

  "rules": [

   {

    "type": "field",

    "ip": [

     "0.0.0.0/8",

     "10.0.0.0/8",

     "100.64.0.0/10",

     "127.0.0.0/8",

     "169.254.0.0/16",

     "172.16.0.0/12",

     "192.0.0.0/24",

     "192.0.2.0/24",

     "192.168.0.0/16",

     "198.18.0.0/15",

     "198.51.100.0/24",

     "203.0.113.0/24",

     "::1/128",

     "fc00::/7",

     "fe80::/10"

    ],

    "outboundTag": "blocked"

   }

  ]

 }

}
```



##### 3.配置Nginx

执行下面的命令，开始配置nginx:

```
[root@ss-us ~]# vi /usr/local/nginx/conf/nginx.conf 
```



按i键编辑文件，把内容更改为下面的内容：

需要在域名指定的目录下面添加home/wwwroot/default文件夹

```
server{

  listen 80;

  server_name vps.baccdc.com;

  return 301 https://$server_name$request_uri;

}

    server {

    listen    443;

    server_name vps.baccdc.com;

    ssl   on;

    root  /home/wwwroot/default;

    index index.html index.htm;

    client_max_body_size 20M;

    ssl_certificate  /usr/local/nginx/2911982_vps.baccdc.com_nginx/2911982_vps.baccdc.com.pem;

    ssl_certificate_key /usr/local/nginx/2911982_vps.baccdc.com_nginx/2911982_vps.baccdc.com.key;

    ssl_session_timeout 5m;

    ssl_ciphers ECDHE-RSA-AES128-GCM-SHA256:ECDHE:ECDH:AES:HIGH:!NULL:!aNULL:!MD5:!ADH:!RC4;

    ssl_protocols TLSv1 TLSv1.1 TLSv1.2;

    ssl_prefer_server_ciphers on;

    location /home/wwwroot/default {

    proxy_redirect off;

    proxy_pass [http://127.0.0.1:32286](http://127.0.0.1:32286/); #此IP地址和端口需要和v2ray服务器保持一致，

    proxy_http_version 1.1;

    proxy_set_header Upgrade $http_upgrade;

    proxy_set_header Connection "upgrade";

    proxy_set_header Host $http_host;

  }

}
```



##### 7.重启v2ray、nginx服务

```
systemctl restart v2ray

systemctl restart nginx
```



##### 8.客户端配置json

**客户端目录下面的config.josn文件配置**

如果你通过Json文件配置，则客户端的json配置内容：

```
{

 "log": {

  "loglevel": "warning"

 },

 "inbound": {

  "port": 1080,

  "listen": "127.0.0.1",

  "protocol": "socks",

  "settings": {

   "auth": "noauth",

   "udp": false

  }

 },

 "inboundDetour": [

  {

    "port": 8128,

    "listen": "127.0.0.1",

    "protocol": "http",

    "settings": {}

  }

 ],

 "outbound": {

  "protocol": "vmess",

  "settings": {

   "vnext": [{

    "address": "hi.v2ray.com",

    "port": 443,

    "users": [{ 

      "id": "0c67ca68-63ad-40c5-898e-9cf1925c8694",

      "level": 1,

      "alterId": 64,

      "security": "aes-128-gcm"

    }]

   }]

  },

  "streamSettings":{

    "network": "ws",

    "security": "tls",

    "tlsSettings": {

      "serverName": "hi.v2ray.com"

    },

    "wsSettings": {

      "path": "/etc/nginx/html"

    }

  },

  "tag": "forgin"

 },

 "outboundDetour": [

  {

    "protocol": "freedom",

    "settings": {},

    "tag": "direct"

  }

 ],

 "routing": {

  "strategy": "rules",

  "settings": {

    "domainStrategy": "IPIfNonMatch",

    "rules": [

      {

        "type": "chinaip",

        "outboundTag": "direct"

      },

     {

        "type": "chinasites",

        "outboundTag": "direct"

      },

      {

       "type": "field",

       "ip": [

          "0.0.0.0/8",

          "10.0.0.0/8",

          "100.64.0.0/10",

          "127.0.0.0/8",

          "169.254.0.0/16",

          "172.16.0.0/12",

          "192.0.0.0/24",

          "192.0.2.0/24",

         "192.168.0.0/16",

          "198.18.0.0/15",

          "198.51.100.0/24",

          "203.0.113.0/24",

          "::1/128",

		  "fc00::/7",

          "fe80::/10"

        ],

        "outboundTag": "direct"

      }

    ]

  }

 },

 "policy": {

  "levels": {

   "0": {"uplinkOnly": 0}

  }

 }

}
```

**5.客户端界面配置**



### **以这个为准**



##### 客户端配置

##### 服务器v2ray配置文件

```
{

 "log" : {

  "access": "/var/log/v2ray/access.log",

  "error": "/var/log/v2ray/error.log",

  "loglevel": "warning"

 },

 "inbound": {

  "port": 10000, //(此端口与nginx配置相关)

  "listen": "127.0.0.1",

  "protocol": "vmess",

  "settings": {

   "clients": [

​    {

​     "id": "461aad1f-687c-4188-9abc-80073a618ca3", //你的UUID， 此ID需与客户端保持一致

​     "level": 1,

​     "alterId": 64 //此ID也需与客户端保持一致

​    }

   ]

  },

  "streamSettings":{

   "network": "ws",

   "wsSettings": {

​      "path": "/ray" //与nginx配置相关

   }

  }

 },

 "outbound": {

  "protocol": "freedom",

  "settings": {}

 },

 "outboundDetour": [

  {

   "protocol": "blackhole",

   "settings": {},

   "tag": "blocked"

  }

 ],

 "routing": {

  "strategy": "rules",

  "settings": {

   "rules": [

​    {

​     "type": "field",

​     "ip": [

​      "0.0.0.0/8",

​      "10.0.0.0/8",

​      "100.64.0.0/10",

​      "127.0.0.0/8",

​      "169.254.0.0/16",

​      "172.16.0.0/12",

​      "192.0.0.0/24",

​      "192.0.2.0/24",

​      "192.168.0.0/16",

​      "198.18.0.0/15",

​      "198.51.100.0/24",

​      "203.0.113.0/24",

​      "::1/128",

​      "fc00::/7",

​      "fe80::/10"

​     ],

​     "outboundTag": "blocked"

​    }

   ]

  }

 }

}
```

##### **v2ray的JSON配置文件, 支持单行注释//， 和多行注释/\* / \***

##### ***\*上面的服务器配置文件也简单注释说明，关于nginx相关的后台会介绍**



**v2ray 客户端配置文件**

```
{

 "log": {

  "loglevel": "warning"

 },

 "inbound": {

  "port": 1080,

  "listen": "127.0.0.1",

  "protocol": "socks",

  "settings": {

   "auth": "noauth",

   "udp": false

  }

 },

 "inboundDetour": [

  {

​    "port": 8123,

​    "listen": "127.0.0.1",

​    "protocol": "http",

​    "settings": {}

  }

 ],

 "outbound": {

  "protocol": "vmess",

  "settings": {

   "vnext": [{

​    "address": "test.v2ray.com", // 服务器地址，请修改为你自己的服务器 ip 或域名

​    "port": 443, // 服务器端口

​    "users": [{ 

​      "id": "461aad1f-687c-4188-9abc-80073a618ca3", //你的UUID， 此ID需与服务端保持一致

​      "level": 1,

​      "alterId": 64, //此ID也需与客户端保持一致

​      "security": "aes-128-gcm"

​    }]

   }]

  },

  "streamSettings":{

​    "network": "ws",

​    "security": "tls",

​    "tlsSettings": {

​      "serverName": "test.v2ray.com" //此域名是你服务器的域名

​    },

​    "wsSettings": {

​      "path": "/ray" //与服务器配置及nginx配置相关

​    }

  },

  "tag": "forgin"

 },

 "outboundDetour": [

  {

​    "protocol": "freedom",

​    "settings": {},

​    "tag": "direct"

  }

 ],

 "routing": { //此路由配置是自动分流， 国内IP和网站直连

  "strategy": "rules",

  "settings": {

​    "domainStrategy": "IPIfNonMatch",

​    "rules": [

​      {

​        "type": "chinaip",

​        "outboundTag": "direct"

​      },

​      {

​        "type": "chinasites",

​        "outboundTag": "direct"

​      },

​      {

​        "type": "field",

​        "ip": [

​          "0.0.0.0/8",

​          "10.0.0.0/8",

​          "100.64.0.0/10",

​          "127.0.0.0/8",

​          "169.254.0.0/16",

​          "172.16.0.0/12",

​          "192.0.0.0/24",

​          "192.0.2.0/24",

​          "192.168.0.0/16",

​          "198.18.0.0/15",

​          "198.51.100.0/24",

​          "203.0.113.0/24",

​          "::1/128",

​          "fc00::/7",

​          "fe80::/10"

​        ],

​        "outboundTag": "direct"

​      }

​    ]

  }

 },

 "policy": {

  "levels": {

   "0": {"uplinkOnly": 0}

  }

 }

}
```



**Nginx 配置**

linux 下的nginx安装就不介绍了， 不清楚的， 可以google 一下

以下是nginx 部分配置， 当然此配置不影响你现在有nginx服务， 只是添加了一个 location /ray.



```
server {

  \# SSL configuration

  listen 443 ssl http2 default_server;

  listen [::]:443 ssl http2 default_server;

  ssl_certificate /ssl.pem; #你的ssl证书， 如果第一次，可能还需要自签一下，

  ssl_certificate_key /ssl.key; #你的ssl key



  root /var/www/html;



  \# Add index.php to the list if you are using PHP

  index index.html index.htm index.nginx-debian.html;



  server_name test.v2ray.com; #你的服务器域名



  location /ray { #/ray 路径需要和v2ray服务器端，客户端保持一致

​    proxy_redirect off;

​    proxy_pass [http://127.0.0.1:10000](http://127.0.0.1:10000/); #此IP地址和端口需要和v2ray服务器保持一致，

​    proxy_http_version 1.1;

​    proxy_set_header Upgrade $http_upgrade;

​    proxy_set_header Connection "upgrade";

​    proxy_set_header Host $http_host;

  }

}
```

关于域名ssl 证书，使用certbot自动签一个let's encrypt证书就行了， 很简单，参考链接: https://certbot.eff.org/

成功后， 在crontab 中添加一条任务计划每三个月执行一次，因为let's encrypt证书三个月过期，



0 0 15 */3 * /root/certbot/certbot-auto renew #在3，6，9，12月份的15号零点零分执行更新

v2ray 客户端的使用

v2ray 客户端主要还在windows上使用， 需要手动编辑config.json文件， 好像还不支持多服务器配置(好久没用了，不知道现在是否可以)

推荐使用界面化v2rayN https://github.com/2dust/v2rayN, 在release页面下载一个v2rayN.exe放在 v2ray客户端文件夹里就行了。

v2rayN使用websocket（ws)时一点需要注意，伪装域名/其选项，应该如下填写





总结

v2ray 的配置相对于ss(ssr)还是复杂一点，其中还涉及到nginx的使用，及ssl证书管理等， 也许需要多一点时间和精力去了解一下， 多看看， 使用效果来说，基本和ss(ssr)差别不大，最主要还是跟服务器相关，相对来说更稳定一些，自从小鸡被放出来后， 就一直使用v2ray，还没有再被墙， 哈哈。
