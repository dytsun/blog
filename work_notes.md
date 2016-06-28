### Work Notes

1. codding中clone一个项目选择SSH地址，提交代码是则不需要输入用户名和密码。

2. 复制之前项目中的bower_components代码时，若bower中插件有改动过，不能执行bower install，否则改动后的代码会被覆盖。

3. angular项目中引用插件，需要在index.module.js中注册插件。

4. angular项目中新建一个模块：

 > 新建模块文件，在html中配置class选择器外层并在css外层中写入，js中配置controller。

 > 在index.route.js中加入路由。
 
 > 在侧边栏菜单中配置模块地址入口。
 
 > translation.js文件中配置中英文翻译。
 
 > cmd中执行gulp serve。

5. 网页打印，@media print中设置打印页面的css
  
  > 横向打印设置 @page {
  size: A4 portrait;
}
6. angular页面传参：
  > 在index.route页面中配置url参数比如：url:'/demo/:code'.
  
  > 用$state.params.code获取参数code.

7. Coding 上 clone一个项目：
  > git clone SSh地址（HTTPS地址需要输入账号与密码，SSH地址不需要）

  > npm install --registry = https://registry.npm.taobao.org (使用淘宝镜像安装包文件)
  
  > bower install (下载包文件)
  
  >gulp serve 运行
  
8. 本地环境不能直接运行php文件，比如浏览器版本过低提示文件，本地不能访问。
