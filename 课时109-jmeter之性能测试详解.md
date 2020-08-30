**课时109-jmeter之性能测试详解**

**Jmerer加到环境变量的步骤：**
1.创建JMETER_HOME,加C:\apache-jmeter-4.0
2.CLASSPATH里面加:
CLASSPATH=%JMETER_HOME%\lib\ext\ApacheJMeter_core.jar; %JMETER_HOME%\lib\jorphan.jar;  
3.path环境变量里面加:
  %JMETER_HOME%/bin;
4.jmeter测试

在cmd中:jmeter -v


**Jmeter生成性能测试报告**
1.修改配置文件jmeter.properties(或者不需要修改，直接是默认的)
  jmeter.save.saveservice.output_format=csv
2.到脚本目录下，直接执行
  cd C:\apache-jmeter-4.0\TestSuite\script
  jmeter -n -t HTTP请求.jmx -l test.jtl -e -o c:/result


**permon插件的应用：**
1.下载permon的插件
2.下载ServerAgent-2.2.1,并且解压
3.监听器中添加permon
4.启动serverAgent的插件,监听端口的4444
5.点击默认点击localhost(也就是本机)


**模板的定制：**
C:\apache-jmeter-4.0\bin\report-template