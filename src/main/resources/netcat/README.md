# 简单例子

1. 配置flume-conf.properties。配置详情查看flume-conf.properties文件。

2. 启动flume agent命令。当一个Flume进程启动时需要说明启动哪个agent，包含--conf=<conf-dir> , 该例子选择Flume在控制台打印日志。<br/>
<code> $ bin/flume-ng agent --conf conf --conf-file conf/flume-conf.properties --name a1 -Dflume.root.logger=INFO,console</code>

3. 发送event到Flume控制台。<br/>
<code> $ telnet localhost 44444 </code> 

4. 参考资料：
 - http://blog.csdn.net/zhouzme/article/details/46461177 Centos7安装telnet 
 - http://blog.csdn.net/anzhuangguai/article/details/52680367 netcat介绍
 - http://www.cnblogs.com/swordfall/p/8095213.html 上述例子来自该链接的 3.1.2 一个简单示例
 
 



