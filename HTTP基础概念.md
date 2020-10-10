# HTTP基础概念

## 请求

请求动词 路径加查询参数  协议名/版本

Host: 域名或IP

accept:表示我想接受什么

content-Type: 请求体的格式

回车

请求体

## 响应体

协议名/版本 状态码 状态字符串

content-Type:响应体的格式

回车

响应体

## 用node.js设置响应

## 设置响应状态码

response.statusCode = 200

## 设置响应头

response.setHeader("Content-Type",'text/html');

## 设置响应体

response.write('内容')

可追加内容

