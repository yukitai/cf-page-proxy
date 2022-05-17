# CloudFlare Pages 反代

使用CloudFlare Pages，反代任何网站

## 简单部署教程

1.下载或是Fork本仓库

2.修改`_worker.js`中第五行的`url.hostname`为你需要反代的网址

3.打开Cloudflare Dashboard，进入Pages管理页面，选择创建项目，如果在第一步中选择的是fork本仓库，则选择1`Connect to Git`，如果第一步中选择的是下载本仓库则选择2`Direct Upload`
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/1.jpg?raw=true)


### 绑定自定义域名

1.进入Cloudflare Pages管理页面，选择刚刚创建的Pages项目，点击名称进入项目设置页面
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/2.jpg?raw=true)

2.选择页面中的`自定义域`
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/3.jpg?raw=true)

3.选择`设置自定义域`
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/4.jpg?raw=true)

4.在页面中输入需要绑定的域名，并点击继续，这里的域名可以是子域名
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/5.jpg?raw=true)

5.在设置方法中选择`开始cname设置`
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/6.jpg?raw=true)

6.按照页面给出的说明去DNS服务提供商处修改DNS解析记录，即可完成自定义域名绑定
![](https://github.com/xyTom/cf-page-func-proxy/blob/images/images/7.jpg?raw=true)
