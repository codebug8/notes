jenkins
==============================

Jenkins是一个用Java编写的开源的持续集成工具。在与Oracle发生争执后，项目从Hudson项目复刻。

Jenkins提供了软件开发的持续集成服务。它运行在Servlet容器中（例如Apache
Tomcat）。它支持软件配置管理（SCM）工具（包括AccuRev
SCM、CVS、Subversion、Git、Perforce、Clearcase和RTC），可以执行基于Apache
Ant和Apache
Maven的项目，以及任意的Shell脚本和Windows批处理命令。Jenkins的主要开发者是川口耕介。Jenkins是在MIT许可证下发布的自由软件。

可以通过各种手段触发构建。例如提交给版本控制系统时被触发，也可以通过类似Cron的机制调度，也可以在其他的构建已经完成时，还可以通过一个特定的URL进行请求。

.. toctree::
    :glob:

    *
