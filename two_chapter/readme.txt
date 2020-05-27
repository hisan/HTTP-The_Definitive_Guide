2020-05-26 杭州
第二章 URL与资源 

URL：因特网资源的标准化名称。

URN:资源位置发生移动后也能被访问，即，资源的访问性不受到资源位置的影响。

URI:URL作为URI的子集





http://www.google.com/pub/a.vedio

rst://www.linux.org/pub/a.vedio

ftp://10.6.121.46/ios/linux.ios





URL语法：
<scheme>://<user>:<password>@<host>:<port>/<path>;<params>?<query>#<frag>
协议：用户(某些资源访问时需要的用户名)：密码(用户名后面可能需要包含的密码，中间由冒号:分隔)

主机:端口:路径:参数:查询:片段




参数组件:
	1.使用;将参数与URL其余部分分隔开来。
	
	2.查询组件：https://www.baidu.com/s?ie=utf-8&f=8&rsv_bp=1&rsv_idx=1&tn=baidu
		2.1 对于 ie=utf-8&f=8&rsv_bp=1&rsv_idx=1&tn=baidu，就是一个查询组件
		
	3.查询字符串以"名/值"来组织，"名/值"间以"&"分隔
	
	4.片段
		为了引用部分资源或资源的一个片段，使用片段组件来表示
			https://www.baidu.com/#ie=UTF-8&wd=%E7%99%BE%E5%BA%A6
			
		但是，不要误解，HTTP服务其通常只处理整个对象，而不是对象的片段，客户端不能将片段传送给服务器。
		浏览器从服务器获得了整个资源之后，会根据片段来显示你感兴趣的那一部分。
		(注意描述：客户端、浏览器、服务器)

缩略形式的URL:可以针对于当前的URL来解释的URl  
	比如 
		https://www.baidu.com/index.html
		
		而index.html中有一个链接引用./login.html
		
