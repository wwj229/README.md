# 管理员配置
# 前言

## Jenkins服务

搭建jenkins实现代码的自动构建、测试、集成部署。

一般流程是，写好自己任务的代码，然后通过git提交，然后将整个模块代码打成war/jar包，然后放入服务器测试运行；如果出现bug，必须由代码编写人员重新审查，排错，重新git提交，重新打包，重新测试。总之就是特别麻烦。

jenkins可以在每个人git代码后，自动的检测到代码的变动，然后自动的打包，测试，提交。出现问题也可以通过发邮件的提醒。

首先，先运行jenkins，jenkins的安装包以war包的形式存在，直接运行war包就可以运行。


## 环境

<ul>
    <li>Jenkins 2.138.2</li>
    <li>CentOS release 6.7</li>
    <li>JDK1.8</li>
    <li>Tomcat 8</li>
    <li>Maven 3.3.9</li>
    <li>远程仓库托管Gitlab 8.17.3</li>
</ul>
