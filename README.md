
## **1.跨平台即时通讯系统（Go，C#，JS，Kotlin，Gin，Vue）**
本科毕业设计
###  1.1 简介
本课题使用WebSocket和SignalR来实现一个简单的跨平台实时通讯应用。该应用允许用户在Web浏览器或Android App上进行实时聊天，支持私聊，群聊，广播，发送文本及图片消息以及传输文件。同时课题也实现了一套流式数据传输的演示程序，以模拟物联网系统中需要处理流式数据的应用场景，如智慧医疗系统中对患者生命体征数据的监控。
###  1.2 技术细节
- 语言及框架：
    - C#，Go，Kotlin，JavaScript
    - .NET WebAPI，Gin，Vue，Gorm，MySQL，JWT
- 服务器搭建：
    - 采用前后端分离的架构构建。
    - 服务器使用.NET Web API框架（结合SignalR组件）和Go语言的开源库Gorilla/Websocket两种技术方案分别实现。
    - 使用MySQL存储用户信息，使用JWT进行身份认证与鉴权。
- 客户端实现：
    - Web端使用Vue框架开发，Android使用Kotlin语言开发。
    - 在Web端针对基于SignalR的服务器和基于Go（WebSocket）的服务器分别设计封装了两套不同的通信接口。
    - Web端使用SignalR的JS语言支持与服务器（基于SignalR）通信。使用原生HTML5原生Websocket支持与服务器（基于Go）通信。
    - Android使用Kotlin开发，使用SignalR的Java语言支持与服务器（基于SignalR）通信。

###  1.3 功能演示
- [实时通信系统功能演示视频（点击跳转）](https://www.bilibili.com/video/BV17W4y1t73n)
![video][pic-1.3.0]<br>
- 聊天室：<br>
![聊天室演示图][pic-1.3.1]<br>
- 图片消息：<br>
![图片消息演示图][pic-1.3.2]<br>
- 文件传输：<br>
![文件传输演示图][pic-1.3.3]<br>
- 流式数据传输：<br>
![流式数据传输演示图][pic-1.3.4]<br>

###  1.4 项目仓库
- .NET服务器：<br>
<https://github.com/HaoyuanMa/IM-Api>
- Go服务器：<br>
<https://github.com/HaoyuanMa/IM-Api-go>
- Web客户端：<br>
<https://github.com/HaoyuanMa/IM-Front-Web>
- Android客户端：<br>
<https://github.com/HaoyuanMa/IM-Front-Android>
- 流式数据生成demo：<br>
<https://github.com/HaoyuanMa/IM-DataStreamGenerator-CSharp><br>
<https://github.com/HaoyuanMa/IM-DataStreamGenerator-go>

---

[pic-1.3.0]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/628cfa92-ca9b-430a-92da-7c533fb98834.png
[pic-1.3.1]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/ea520e51-4294-4b9a-a601-43c6d8221aa6.png
[pic-1.3.2]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/ce000332-4e71-41b5-86f7-525382cbf046.png
[pic-1.3.3]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/e8261b77-42b2-425f-8afe-382559d5677e.png
[pic-1.3.4]: https://vkceyugu.cdn.bspapp.com/VKCEYUGU-1682933a-c290-4a19-a517-c44d14df20fc/82f97639-a929-4e4d-851a-ed617c532ae1.png
