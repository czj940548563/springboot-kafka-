# springboot-kafka-
win:
安装zookeeper，并启动，自行百度教程
安装kafka
在kafa目录下的config下配置server.properties
zookeeper.connect=ip:2181

启动kafka（linux的在bin下，把bat改为sh后缀即可）;
/bin/windows 打开命令行
.\kafka-console-consumer.bat  接server.properties的绝对路径

另起一个命令行查看消费者接收的消息:
.\kafka-console-consumer.bat --bootstrap-server ip:9092 --topic hello --from-beginning

启动springboot的启动类即可在IDE的控制台和消费者命令行看到消息。
