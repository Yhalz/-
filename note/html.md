http-srver //使用hs给的ip试
Chrome 远程调试
127.0.0.1 自己
默认使用80端口或者442端口
nslookup baidu.com 域名查询
114.114.114/5.114/5 电信dns服务器地址 

url//统一资源定位服务查询指南
https://www.baidu.com/s    ?wd=hello&srv_spt=1 #5
协议     域名         路径    查询参数          锚点 

锚点不支持中文

请求不同的页面
路径/html  or   路径/css   or ......
路径可以不加后缀

查询同一个页面不同参数
www.baidu.com/s?wd=hi
www.baidu.com/s?wd=hello

curl -v http://baidu.com
curl -s -v http://baidu.com

.com 顶级域名
baidu.com 二级域名
www.baidu.com 三级域名