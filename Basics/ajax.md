# 尚硅谷-AJAX课程

## 原生AJAX

### AJAX简介

AJAX就是异步JS和XML

通过AJAX可以在浏览器中向服务器发送异步请求，无刷新获取数据

AJAX不是新的编程语言，而是一种将现有的标准组合在一起的一种新的方式

### XML简介

1. XML可扩展标记语言

2. XML被设计用来传输和存储数据

3. XML和HTML类似，不同的事，XML中没有预定义标签，全都是自定义标签，用来存储数据

   ```xml
   <student>
       <name>孙悟空</name>
       <age>18</age>
       <gender>男</gender>
   </student>
   ```

### AJAX优缺点

#### 优点

1. 可以无需刷新页面而与服务器端进行通信
2. 允许你根据用户事件来更新部分页面内容

#### 缺点

1. 没有浏览记录，不能回退
2. 存在跨域问题（同源）
3. SEO不友好（爬虫爬不到）

## HTTP协议请求报文与响应文本结构

### 请求报文

格式与参数

```http
请求行		POST	/s?ie=utf-8	HTTP/1.1
请求头		Host:atgui.com
		  Cookie:name=guigu
		  Content-type:application/x-www/form-urlencoded
		  USer-Agent:chrom 83
空行
请求体		(GET请求为空，POST请求体可以不为空)
		  username=admin&password&admin
```

### 响应报文

格式与参数

```http
响应行	HTTP/1.1 200 OK
响应头	(与请求头格式一样)
空行	  
响应体	(返回的结果)
	<html>
	······
	</html>
```

### Chrom查看请求和相应

位置：F12--网络中

#### Headers

包括请求头与响应头（格式key:value)

