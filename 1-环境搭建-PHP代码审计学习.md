# 环境搭建

环境准备：phpstudy（一键搭建PHP环境）+phpstorm(php IDE)+xdebug（动态调试）

下载地址：https://www.xp.cn/download.html  官网的是新版本，用不惯可以找我要老版本。

https://www.jetbrains.com/phpstorm/download/

------

1. 下载完成后安装phpstudy并选择PHP版本后运行，我这里用的是7.2.10,如果你用的版本和我一样，请下载这个版本的xdebug，http://xdebug.org/files/php_xdebug-3.0.4-7.2-vc15-nts.dll 。其他的php版本，请打开导航页面，复制phpinfo页面内容到里面，然后根据提示操作。https://xdebug.org/wizard 是导航页面地址。



<img src="\image-20210803221938772.png" alt="image-20210803221938772" style="zoom:50%;" />

2. 下载xdebug的文件后，移动到你phpstudy的路径下面，我的是D:\phpStudy\PHPTutorial\php\php-7.2.1-nts\ext 。然后编辑D:\phpStudy\PHPTutorial\php\php-7.2.1-nts\php.ini 文件，在最后一行添加	

   zend_extension = D:\phpStudy\PHPTutorial\php\php-7.2.1-nts\ext\php_xdebug-3.0.4-7.2-        vc15-nts.dll

   这里请根据自己的路径和版本号进行改变。然后保存并重启webserver。查看phpinfo页面，搜索“xdebug”关键词，如果出现了所示的内容，则说明配置成功。

   <img src="C:\Users\LY\AppData\Roaming\Typora\typora-user-images\image-20210803223704370.png" alt="image-20210803223704370" style="zoom:50%;" />

3. XDebug环境配置后，我们需要下载PhpStorm来配合使用（具体安装方法百度吧，我这里激活用这个激活码：https://api.kuku.me/tool/jetbrains）。安装完毕，运行PhpStorm，选择“Configure→Settings”，然后选择“Languages&Frameworks→PHP→Debug”，设置调试端口为9000。

   <img src="C:\Users\LY\AppData\Roaming\Typora\typora-user-images\image-20210803224115980.png" alt="image-20210803224115980" style="zoom:50%;" />

4. 
