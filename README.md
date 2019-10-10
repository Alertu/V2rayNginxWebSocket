<p>
    <span style="font-size: 36px;"><strong>安装</strong></span>
</p>
<p>
    3.安装wget
</p>
<p>
    <br/>
</p>
<p>
    digitalocean默认没有安装wget，我们需要自己安装，执行如下命令进行安装：
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">yum -y install wget</span>
</p>
<p>
    4.下载脚本
</p>
<p>
    <br/>
</p>
<p>
    安装完wget之后就可以进行下载操作了，如下：
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">wget https://install.direct/go.sh</span>
</p>
<p>
    5.安装unzip
</p>
<p>
    <br/>
</p>
<p>
    因为centos不支持apt-get，我们需要安装unzip，详见官方说明：
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">yum install -y zip unzip&nbsp;&nbsp;</span>
</p>
<p>
    6.执行安装
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">[michael@centos74 v2ray]$ bash go.sh&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">Installing V2Ray v3.14 on x86_64</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">Downloading V2Ray.</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; % Total&nbsp; &nbsp; % Received % Xferd&nbsp; Average Speed&nbsp; &nbsp;Time&nbsp; &nbsp; Time&nbsp; &nbsp; &nbsp;Time&nbsp; Current</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Dload&nbsp; Upload&nbsp; &nbsp;Total&nbsp; &nbsp;Spent&nbsp; &nbsp; Left&nbsp; Speed</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">100&nbsp; &nbsp;608&nbsp; &nbsp; 0&nbsp; &nbsp;608&nbsp; &nbsp; 0&nbsp; &nbsp; &nbsp;0&nbsp; &nbsp;2229&nbsp; &nbsp; &nbsp; 0 --:--:-- --:--:-- --:--:--&nbsp; 2235</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">100 8482k&nbsp; 100 8482k&nbsp; &nbsp; 0&nbsp; &nbsp; &nbsp;0&nbsp; 2501k&nbsp; &nbsp; &nbsp; 0&nbsp; 0:00:03&nbsp; 0:00:03 --:--:-- 2813k</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">Extracting V2Ray package to /tmp/v2ray.</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">Archive:&nbsp; /tmp/v2ray/v2ray.zip</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp;creating: /tmp/v2ray/v2ray-v3.14-linux-64/</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/geoip.dat&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/geosite.dat&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/readme.md&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp;creating: /tmp/v2ray/v2ray-v3.14-linux-64/systemd/</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/systemd/v2ray.service&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp;creating: /tmp/v2ray/v2ray-v3.14-linux-64/systemv/</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/systemv/v2ray&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/v2ctl&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp;extracting: /tmp/v2ray/v2ray-v3.14-linux-64/v2ctl.sig&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/v2ray&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp;extracting: /tmp/v2ray/v2ray-v3.14-linux-64/v2ray.sig&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/vpoint_socks_vmess.json&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; inflating: /tmp/v2ray/v2ray-v3.14-linux-64/vpoint_vmess_freedom.json&nbsp;&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">PORT:13437</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">UUID:f500ecf5-e135-49c6-9ce2-78eb490d0aa9</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">Created symlink from /etc/systemd/system/multi-user.target.wants/v2ray.service to /etc/systemd/system/v2ray.service.</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">V2Ray v3.14 is installed.</span>
</p>
<p>
    7.相关命令
</p>
<p>
    <br/>
</p>
<p>
    在首次安装完成之后，V2Ray不会自动启动，需要手动运行上述启动命令。而在已经运行V2Ray的VPS上再次执行安装脚本，安装脚本会自动停止V2Ray 进程，升级V2Ray程序，然后自动运行V2Ray。在升级过程中，配置文件不会被修改。
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">## 启动</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">systemctl start v2ray</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">## 停止</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">systemctl stop v2ray</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">## 重启</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">systemctl restart v2ray</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">## 开机自启</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">systemctl enable v2ray</span>
</p>
<p>
    关于软件更新：更新 V2Ray 的方法是再次执行安装脚本！再次执行安装脚本！再次执行安装脚本！
</p>
<p>
    <br/>
</p>
<p>
    3.配置v2ray服务端
</p>
<p>
    假设你的域名是v2ray.com，并将二级域名hi.v2ray.com解析到你的VPS。
</p>
<p>
    <br/>
</p>
<p>
    执行下面的命令，开始配置v2ray:
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">[root@ss-us ~]# vi /etc/v2ray/config.json&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">按i键编辑文件，把内容更改为下面的内容：</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">{</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;log&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;access&quot;: &quot;/var/log/v2ray/access.log&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;error&quot;: &quot;/var/log/v2ray/error.log&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;loglevel&quot;: &quot;warning&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;inbounds&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;port&quot;: 33684,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;listen&quot;: &quot;127.0.0.1&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;vmess&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;clients&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;id&quot;: &quot;0c67ca68-63ad-40c5-898e-9cf1925c8694&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;level&quot;: 1,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;alterId&quot;: 64</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ]</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;streamSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;network&quot;: &quot;ws&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;wsSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;path&quot;: &quot;/etc/nginx/html&quot;//这个地址就是使用一键安装工具生成之后访问到的地址，也就是虚拟目录访问地址</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;outbounds&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;freedom&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;settings&quot;: {},</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;tag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;blackhole&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;settings&quot;: {},</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;tag&quot;: &quot;blocked&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;routing&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;rules&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;field&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;ip&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;0.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;10.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;100.64.0.0/10&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;127.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;169.254.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;172.16.0.0/12&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.0.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.2.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.168.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.18.0.0/15&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.51.100.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;203.0.113.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;::1/128&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fc00::/7&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fe80::/10&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;blocked&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; ]</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">}</span>
</p>
<p>
    <span style="font-size: 36px;"><strong>3.配置Nginx</strong></span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">执行下面的命令，开始配置nginx:</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">[root@ss-us ~]# vi /usr/local/nginx/conf/nginx.conf&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">按i键编辑文件，把内容更改为下面的内容：</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">需要在域名指定的目录下面添加home/wwwroot/default文件夹</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">server{</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; listen 80;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; server_name vps.baccdc.com;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; return 301 https://$server_name$request_uri;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">}</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp;server {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; listen&nbsp; &nbsp; &nbsp; &nbsp;443;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; server_name&nbsp; vps.baccdc.com;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl&nbsp; &nbsp; &nbsp;on;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; root&nbsp; &nbsp;/home/wwwroot/default;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; index&nbsp; index.html index.htm;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; client_max_body_size 20M;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl_certificate&nbsp; &nbsp;/usr/local/nginx/2911982_vps.baccdc.com_nginx/2911982_vps.baccdc.com.pem;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl_certificate_key&nbsp; /usr/local/nginx/2911982_vps.baccdc.com_nginx/2911982_vps.baccdc.com.key;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl_session_timeout 5m;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl_ciphers ECDHE-RSA-AES128-GCM-SHA256:ECDHE:ECDH:AES:HIGH:!NULL:!aNULL:!MD5:!ADH:!RC4;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl_protocols TLSv1 TLSv1.1 TLSv1.2;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ssl_prefer_server_ciphers on;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; location /home/wwwroot/default {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_redirect off;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_pass http://127.0.0.1:32286; #此IP地址和端口需要和v2ray服务器保持一致，</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_http_version 1.1;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_set_header Upgrade $http_upgrade;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_set_header Connection &quot;upgrade&quot;;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_set_header Host $http_host;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">}</span>
</p>
<p>
    <br/>
</p>
<p>
    4.重启v2ray、nginx服务
</p>
<p>
    systemctl restart v2ray
</p>
<p>
    <br/>
</p>
<p>
    systemctl restart nginx
</p>
<p>
    <span style="font-size: 36px;"><strong>客户端配置json</strong></span>
</p>
<p>
    <span style="font-size: 36px;"><strong>客户端目录下面的config.josn文件配置</strong></span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">如果你通过Json文件配置，则客户端的json配置内容：</span><br/>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">{</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;log&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;loglevel&quot;: &quot;warning&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;inbound&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;port&quot;: 1080,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;listen&quot;: &quot;127.0.0.1&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;protocol&quot;: &quot;socks&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;auth&quot;: &quot;noauth&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;udp&quot;: false</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;inboundDetour&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;port&quot;: 8128,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;listen&quot;: &quot;127.0.0.1&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;http&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;settings&quot;: {}</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;outbound&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;protocol&quot;: &quot;vmess&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;vnext&quot;: [{</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;address&quot;: &quot;hi.v2ray.com&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;port&quot;: 443,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;users&quot;: [{&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;id&quot;: &quot;0c67ca68-63ad-40c5-898e-9cf1925c8694&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;level&quot;: 1,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;alterId&quot;: 64,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;security&quot;: &quot;aes-128-gcm&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }]</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; }]</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;streamSettings&quot;:{</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;network&quot;: &quot;ws&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;security&quot;: &quot;tls&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;tlsSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;serverName&quot;: &quot;hi.v2ray.com&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;wsSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;path&quot;: &quot;/etc/nginx/html&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;tag&quot;: &quot;forgin&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;outboundDetour&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;freedom&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;settings&quot;: {},</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;tag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;routing&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;strategy&quot;: &quot;rules&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;domainStrategy&quot;: &quot;IPIfNonMatch&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;rules&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;chinaip&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;chinasites&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;field&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;ip&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;0.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;10.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;100.64.0.0/10&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;127.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;169.254.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;172.16.0.0/12&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.0.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.2.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.168.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.18.0.0/15&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.51.100.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;203.0.113.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;::1/128&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fc00::/7&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fe80::/10&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ]</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &quot;policy&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &quot;levels&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; &nbsp; &quot;0&quot;: {&quot;uplinkOnly&quot;: 0}</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">&nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 255, 0);">}</span>
</p>
<p>
    <span style="font-size: 36px;"><strong><span style="background-color: rgb(255, 0, 0);">5.客户端界面配置</span></strong></span>
</p>
<p>
    <span style="font-size: 36px; background-color: rgb(255, 0, 0);"><b>以这个为准</b></span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">客户端配置</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">服务器v2ray配置文件</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">{</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;log&quot; : {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;access&quot;: &quot;/var/log/v2ray/access.log&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;error&quot;: &quot;/var/log/v2ray/error.log&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;loglevel&quot;: &quot;warning&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;inbound&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;port&quot;: 10000, //(此端口与nginx配置相关)</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;listen&quot;: &quot;127.0.0.1&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;protocol&quot;: &quot;vmess&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;clients&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;id&quot;: &quot;461aad1f-687c-4188-9abc-80073a618ca3&quot;, //你的UUID， 此ID需与客户端保持一致</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;level&quot;: 1,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;alterId&quot;: 64 //此ID也需与客户端保持一致</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; ]</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp;&quot;streamSettings&quot;:{</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;network&quot;: &quot;ws&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;wsSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&quot;path&quot;: &quot;/ray&quot; //与nginx配置相关</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp;}</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;outbound&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;protocol&quot;: &quot;freedom&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;settings&quot;: {}</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;outboundDetour&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;blackhole&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;settings&quot;: {},</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;tag&quot;: &quot;blocked&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;routing&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;strategy&quot;: &quot;rules&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;rules&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;field&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;ip&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;0.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;10.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;100.64.0.0/10&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;127.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;169.254.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;172.16.0.0/12&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.0.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.2.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.168.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.18.0.0/15&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.51.100.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;203.0.113.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;::1/128&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fc00::/7&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fe80::/10&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;blocked&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; ]</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">}</span>
</p>
<p>
    <span style="font-size: 36px;"><strong>v2ray的JSON配置文件, 支持单行注释//， 和多行注释/* / *</strong></span>
</p>
<p>
    <span style="font-size: 36px;"><strong>**上面的服务器配置文件也简单注释说明，关于nginx相关的后台会介绍</strong></span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="font-size: 36px;"><strong>v2ray 客户端配置文件</strong></span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">{</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;log&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;loglevel&quot;: &quot;warning&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;inbound&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;port&quot;: 1080,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;listen&quot;: &quot;127.0.0.1&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;protocol&quot;: &quot;socks&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;auth&quot;: &quot;noauth&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;udp&quot;: false</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;inboundDetour&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;port&quot;: 8123,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;listen&quot;: &quot;127.0.0.1&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;http&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;settings&quot;: {}</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;outbound&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;protocol&quot;: &quot;vmess&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;vnext&quot;: [{</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;address&quot;: &quot;test.v2ray.com&quot;, // 服务器地址，请修改为你自己的服务器 ip 或域名</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;port&quot;: 443,&nbsp; // 服务器端口</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;users&quot;: [{&nbsp;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;id&quot;: &quot;461aad1f-687c-4188-9abc-80073a618ca3&quot;, //你的UUID， 此ID需与服务端保持一致</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;level&quot;: 1,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;alterId&quot;: 64,&nbsp; //此ID也需与客户端保持一致</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;security&quot;: &quot;aes-128-gcm&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }]</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; }]</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;streamSettings&quot;:{</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;network&quot;: &quot;ws&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;security&quot;: &quot;tls&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;tlsSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;serverName&quot;: &quot;test.v2ray.com&quot; //此域名是你服务器的域名</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;wsSettings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;path&quot;: &quot;/ray&quot; //与服务器配置及nginx配置相关</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;tag&quot;: &quot;forgin&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;outboundDetour&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;protocol&quot;: &quot;freedom&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;settings&quot;: {},</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;tag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;routing&quot;: { //此路由配置是自动分流， 国内IP和网站直连</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;strategy&quot;: &quot;rules&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;settings&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;domainStrategy&quot;: &quot;IPIfNonMatch&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &quot;rules&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;chinaip&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;chinasites&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;type&quot;: &quot;field&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;ip&quot;: [</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;0.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;10.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;100.64.0.0/10&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;127.0.0.0/8&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;169.254.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;172.16.0.0/12&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.0.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.0.2.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;192.168.0.0/16&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.18.0.0/15&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;198.51.100.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;203.0.113.0/24&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;::1/128&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fc00::/7&quot;,</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;fe80::/10&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ],</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &quot;outboundTag&quot;: &quot;direct&quot;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; ]</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; },</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &quot;policy&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &quot;levels&quot;: {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &quot;0&quot;: {&quot;uplinkOnly&quot;: 0}</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">}</span>
</p>
<p>
    <span style="font-size: 36px;"><strong>Nginx 配置</strong></span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">linux 下的nginx安装就不介绍了， 不清楚的， 可以google 一下</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">以下是nginx 部分配置， 当然此配置不影响你现在有nginx服务， 只是添加了一个 location /ray.</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">server {</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; # SSL configuration</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; listen 443 ssl http2 default_server;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; listen [::]:443 ssl http2 default_server;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; ssl_certificate /ssl.pem; #你的ssl证书， 如果第一次，可能还需要自签一下，</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; ssl_certificate_key /ssl.key; #你的ssl key</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; root /var/www/html;</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; # Add index.php to the list if you are using PHP</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; index index.html index.htm index.nginx-debian.html;</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; server_name test.v2ray.com; #你的服务器域名</span>
</p>
<p>
    <br/>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; location /ray { #/ray 路径需要和v2ray服务器端，客户端保持一致</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_redirect off;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_pass http://127.0.0.1:10000; #此IP地址和端口需要和v2ray服务器保持一致，</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_http_version 1.1;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_set_header Upgrade $http_upgrade;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_set_header Connection &quot;upgrade&quot;;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; &nbsp; &nbsp; proxy_set_header Host $http_host;</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">&nbsp; &nbsp; }</span>
</p>
<p>
    <span style="background-color: rgb(255, 0, 0);">}</span>
</p>
<p>
    关于域名ssl 证书，使用certbot自动签一个let&#39;s encrypt证书就行了， 很简单，参考链接: https://certbot.eff.org/
</p>
<p>
    成功后， 在crontab 中添加一条任务计划每三个月执行一次，因为let&#39;s encrypt证书三个月过期，
</p>
<p>
    <br/>
</p>
<p>
    0 0 15 */3 * /root/certbot/certbot-auto renew&nbsp; #在3，6，9，12月份的15号零点零分执行更新
</p>
<p>
    v2ray 客户端的使用
</p>
<p>
    v2ray 客户端主要还在windows上使用， 需要手动编辑config.json文件， 好像还不支持多服务器配置(好久没用了，不知道现在是否可以)
</p>
<p>
    推荐使用界面化v2rayN https://github.com/2dust/v2rayN, 在release页面下载一个v2rayN.exe放在 v2ray客户端文件夹里就行了。
</p>
<p>
    v2rayN使用websocket（ws)时一点需要注意，伪装域名/其选项，应该如下填写
</p>
<p>
    <br/>
</p>
<p>
    /ray;test.v2ray.com&nbsp; #请更换为自己的相关配置
</p>
<p>
    其它配置请参考截图 https://i.loli.net/2018/07/08/5b41ff02d15a3.png
</p>
<p>
    <br/>
</p>
<p>
    总结
</p>
<p>
    v2ray 的配置相对于ss(ssr)还是复杂一点，其中还涉及到nginx的使用，及ssl证书管理等， 也许需要多一点时间和精力去了解一下， 多看看， 使用效果来说，基本和ss(ssr)差别不大，最主要还是跟服务器相关，相对来说更稳定一些，自从小鸡被放出来后， 就一直使用v2ray，还没有再被墙， 哈哈。
</p>
<p>
    后续再介绍一下v2ray 免流，地址: v2ray 免流 配置
</p>
<p>
    <br/>
</p>
