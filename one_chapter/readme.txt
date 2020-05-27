2020-05-23 杭州
第一章 HTTP概述

MIME type (本来是Multiple internet Mail Extention)  标记多媒体内容


URL:	一台特定服务器上某资源的特定位置。(明确说明如何从一个精确的、固定的位置获取资源)


URN：统一资源名(不限空间访问资源)


事务：一个HTTP事务由一条请求命令(client--->server)和一个响应结果组成(server--->client)

命令：请求方法
	常见5种请求方法:
	
		GET			从服务器向客户端发送命名资源
		PUT			将来自客户端的数据存储到一个命名的服务器资源中去
		DELETE		从服务器中删除命名资源
		POST		将客户端数据发送到一个服务器网关应用程序
		HEAD		仅发送命名资源响应中的HTTP首部
		

状态码(由三个数字组成)：每条HTTP响应报文返回时都会携带一个状态码。

报文：HTTP报文都是纯文本。
	1.1 请求报文
		GET	/test/index.html HTTP/1.0		起始行
		Accept:text/*						首部
		Accept-Language: en,fr				
		
	1.2 响应报文	
		HTTP/1.0 200 OK					       起始行
		Content-type: text/plain               首部
		Content-length: 19                     
		
		Hi,I'm a message!                      主体(主题可以包含任意二进制数据：图片、视频、音乐、软件程序)
		
		
		
	
	client---------请求报文-------->server
	
	server---------响应报文-------->client
	
	
HTTP/1.1是目前正在使用的HTTP版本


其他的重要程序：
	代理：
		
	缓存：(一种特殊的HTTP代理服务器，可将经过代理传送常用的文档复制保存起来)
		HTTP的仓库，使常用页面的副本可以保存在离客户端更近的地方
		
	网关：(通常用于将HTTP流量转换成其他的协议)
		连接其他应用程序的特殊web服务器
		
	隧道：(HTTP隧道通常用来在一条或多条HTTP连接上转发非HTTP数据，转发时不会窥探数据)   主要是承载SSL报文
		对HTTP通信报文进行盲转发的特殊代理
	
	Agent代理：(代表用户发起HTTP请求的客户端程序)===web浏览器
		发起自动HTTP请求的半智能web客户端
		
		
	
	
	
	
	
	
	
	
	