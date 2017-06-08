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

9. 扫描二维码判断微信，ios，Android跳转：
  > if (ua.indexOf('micromessenger') > 0) { //需对所有 android 系统 UA 信息进行判断

  > document.write('微信中无法直接下载 App，请点击右上角菜单，选择"在浏览器中打开"下载 App 。');
  
  > } else if (ua.indexOf('iphone') > 0) { //需对所有 ios 系统 UA 信息进行判断
  
  >  window.location.href = ios_down_url;
  
  > } else if (ua.indexOf('android') > 0) {
  
  >   window.location.href = android_down_url;
  
  > }
  
10. ie8下css:background-size:cover不兼容，解决办法：
  > filter: progid:DXImageTransform.Microsoft.AlphaImageLoader(src='images/banner1.png',sizingMethod='scale');

11. win10 配置git环境，coding git代码托管：
  > (1)下载安装git

  > (2)双击打开git/git-bash程序

  > (3)在git-bash界面中，输入git config --global user.name "me",运行。

  > (4)在git-bash界面中，输入git congig --global user.email "me@.com"。

  > (5)生成一个新的SSH公钥，在git-bash界面中，输入ssh-keygen -t rsa -C "me@.com",此时在C：/user/administrator中生成.ssh文件。

  > (6)在git-bash界面中输入ssh -t git@git.coding.net,测试建立链接会要求信任主机。

  > (7)在C：/user/administrator中生成.ssh文件，打开 id_rsa.pub 文件（或执行 $cat id_rsa.pub ），复制其中全部内容，添加到账户“SSH   公钥”页面 中，公钥名称可以随意起名字。完成后点击“添加”，然后输入密码或动态码即可添加完成。
  
  > (8)配置参考https://coding.net/help/doc/git/ssh-key.html
  
12. 管理员身份删除文件夹
  > (1)打开管理员命令行界面
  
  > (2)rd /s/q C:\Windows.old，回车
  
13. chrome浏览器屏蔽input默认提示：
  > form后加novalidate属性。
  
  > input后加 autocomplete="off"属性，阻止autocomplete行为。
  
14. win10添加开机启动项：
  > 打开文件夹 C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp 直接复制到地址栏里面打开即可。
  
  > 复制启动项的快捷方式，粘贴到启动文件夹中。
  
  > 命令行中运行 msconfig.查看启动项是否添加成功。
  
15. 闭包作用域：
  
  > for (var i=1; i<=5; i++) {
  
  >   let j = i; // 呀，给闭包的块儿作用域！
  
  >   setTimeout( function timer(){
  
  >     console.log( j );
  
  >   }, j*1000 );
  
  > }  //每隔1秒输出1，2，3，4，5
  
16. npm镜像默认修改：

  > 打开C:\Users\Administrator中.npmrc文件
  
  > 加入下面内容: registry = http://registry.npm.taobao.org 即：替换为淘宝镜像。
  
  
  
  
  
  
