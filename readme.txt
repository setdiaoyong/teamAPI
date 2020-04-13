按照github：https://github.com/OfficeDev/msteams-app-lms-meetings项目下说明设置应用ID授权，其中到Redirect URIs ，除了http://localhost:3000/，还要增加自己的部署所用的https://网址到Redirect URIs，不然可能子账号登录会报Redirect URIs不相符的错（需要ssl安全认证的https://域名，没有走Render在线编译部署）

基于2020年4月10日github最新版，编译打包
1、用notepad++ ，或其他IDE，分别打开build\static\js\main.b09a1c35.chunk.js和build\static\js\main.b09a1c35.chunk.js.map
2、在分别在以上两个文件搜索 {授权appID} ，将 {授权appID}  连 { }挂号一起替换成至自己设置好的app ID
3、上传到支持静态博客的空间，部署域名后登录子账号，创建一下team的meeting，就可以了。
4、已验证，能在国内免费空间coding.net部署成功
