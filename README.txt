按照我的博客http://blog.xbreeding.com/index.php/archives/4/说明设置应用ID授权，其中到Redirect URIs ，除了http://localhost:3000/，还要增加自己的部署所用的https://网址到Redirect URIs，不然可能子账号登录会报Redirect URIs不相符的错（需要ssl安全认证的https://域名）

基于2020年4月10日原项目github最新版，编译打包

1、拉取到自己的github，改成自己的github用户名.github.io，分别打开static\js\main.b09a1c35.chunk.js和build\static\js\main.b09a1c35.chunk.js.map 分别搜索 {授权appID} ，将 {授权appID}  连 { }挂号一起替换成至自己设置好的app ID

3、参考https://blog.csdn.net/yuexianchang/article/details/53431703设置githubpage，用githubpage就行，部署后，登录子账号，创建一下team的meeting，就可以了。

4、已验证，该静态文件能在国内免费空间coding.net部署成功：我部署的欢迎注册https://h0hyvx.coding-pages.com

下载静态文件，点击绿色图标，下载zip压缩包。
