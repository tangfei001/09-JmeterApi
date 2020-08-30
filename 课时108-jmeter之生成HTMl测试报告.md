**课时108-jmeter之生成HTMl测试报告**




# 01:搭建测试环境-详见搭建测环境  #

   注意:将创建好的build.xml文件放到jmeter的目录tests中去

## 02:目录创建 ##
   
   01:安装jmeter时在根目录创建 tests 目录

   02:在tests目录中创建 script report目录

   03:在report目录中创建 html jtl目录

 ###  03:自动发送邮件问题总结  ###

    1:自动发送邮件需要三个jar包,分别是: activation,jar,
      commons-email-1.2.jar
       mail.jar
      这三个文件放在ant的lib目录下

    2:Exception resding response timeout stack jire-JRE

    3:authoration,401,403
