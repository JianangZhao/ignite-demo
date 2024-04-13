login Ignite 中文社区

https://ignite-service.cn/doc/java/QuickStartGuide.html#_1-5-%E8%BF%9B%E4%B8%80%E6%AD%A5%E7%9A%84%E7%A4%BA%E4%BE%8B

下载最新的Ignite cache: Download - Apache Ignite
    解压缩下载的安装包apache-ignite-2.16.0-src\bin\ignite.bat
    启动ignite server端
    ignite.sh|bat默认会使用config/default-config.xml这个配置文件启动节点。
        cd {IGNITE_HOME}\bin\
        启动节点 ignite.bat ..\examples\config\example-ignite.xml 打印日志如下
            [18:01:11] Ignite node started OK (id=fa411460)
            [18:01:11] Topology snapshot [ver=1, locNode=fa411460, servers=1, clients=0, state=ACTIVE, CPUs=12, offheap=6.4GB, heap=1.0GB]

        新建窗口 启动另一节点 ignite.bat ..\examples\config\example-ignite.xml 打印日志如下
            [18:02:13] Ignite node started OK (id=dbf338ef)
            [18:02:13] Topology snapshot [ver=2, locNode=dbf338ef, servers=2, clients=0, state=ACTIVE, CPUs=12, offheap=13.0GB, heap=2.0GB]


添加pom依赖

创建测试工程

启动测试 控制台会打印下面的信息

>> Executing the compute task
   Node ID: dbf338ef-bddd-4f4d-b9d2-5f7d8bccf006
   OS: Windows 11   JRE: Java(TM) SE Runtime Environment
>> Hello World!
