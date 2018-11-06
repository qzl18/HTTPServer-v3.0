HTTPServer+WebFrame
HTTPServer功能:
    1.获取HTTP请求
    2.解析HTTP请求
    3.将请求内容发给WebFrame
    4.将数据组织为Response格式发送给客户端

WebFrame功能:
    1.从HTTPServer接收具体请求
    2.判断请求网页或者数据,根据请求调用函数处理
    3.将网页或者数据发送给HTTPServer
升级点:
    1.采用了HTTPServer与应用程序分离,两个功能模块独立,降低耦合度
    2.数据的处理单独调用函数完成
    3.两者的配合使用进程间通信(套接字就可以)


