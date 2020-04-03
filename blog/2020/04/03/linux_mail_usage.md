#Linux mail


mail 命令是 Linux 下一个非常轻巧的交互式的命令行邮件客户端，基于 Berkeley Mail 8.1，提供 MIME、MAP、POP3、SMTP 和 S/MIME 等扩展

mail 默认是调用本机 MTA 发送邮件的，这意味着需要在本机上安装 sendmail 或 postfix 或 exim 或…，配置比较麻烦，而且会带来不必要的资源占用。

通过修改配置文件，可以达到不使用 sendmail 而用外部 smtp 服务器发送邮件的目的。

###命令介绍
命令名称 mail/mailx

* 基本语法
常用选项的简化语法可能包括：mail [-s subject] [-c cc-addr] to-addr . . .

* 功能描述
发送和接收网络邮件

###命令选项

| option | usage |
| :----   |  :---- |
| -b address | 指定密件副本的收信人地址 |
| -c address	| 指定副本的收信人地址 |
| -f [file]	| 读取指定邮件文件中的邮件|
| -i	| 忽略终端发出的信息|
| -I	| 使用互动模式|
| -n	| 启动时禁止读取 /etc/mail.rc|
| -N	| 阅读邮件时，不显示邮件的标题|
| -s | subject	指定邮件的主题|
| -t	| 要发送的消息应包含带有 To:、Cc:、或 Bcc: 字段的消息头，在命令行上指定的收件人将被忽略。|
| -u | user	读取指定用户的邮件|
| -v	| 执行时，显示详细的信息|
| -V | 显示版本信息并退出|


