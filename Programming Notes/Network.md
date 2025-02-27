# HTTP/HTTPS

##### *HTTP(Hyper-Text-Transfer-Protocal-Secure)*

### Status Code

- ##### 2xx Success 200 OK, 204 No Content 响应头没有body数据 206 Partial Content 分块下载，非返回全部
- ##### 3xx Redirect 301 Moved Permanently 资源不存在 302 Found 临时重定向 资源存在 需要其他url访问 304 Not Modified 缓存重定向  用于缓存控制
- ##### 4xx Client Error 请求报文错误 服务端无法处理 400 Bad Request 请求报文错误 403 Forbidden 404 Not Found
- ##### 5xx Server Error 服务端内部错误 500 Internal Server Error 服务器未知错误 501 Not Implemented 功能不支持 502 Bad Gateway  503 Serveice Unavaliable 服务器忙
- ##### 1xx Processing wating for rest operation

### HTTP常见字段
- *content length:* 表示服务器回应数据长度
- *connection:* http 长连接 keep-alive 只要任意一端不断开则TCP保持连接
- *Content-Type: *用于服务器回应 告诉客户端数据格式 text/html Charset=utf-8 请求时可以使用Accept：*/*表示数据接受格式
- TCP 三次握手建立连接 四次挥手断开连接
-


### GET/POST

- ##### GET
    - 从服务器获取指定资源(文本 页面 图片 视频) 参数写在URL 只支持ASCII字符 
    - 有长度限制 基于浏览器 或者中间件 推荐1000-2000 字符 or more
