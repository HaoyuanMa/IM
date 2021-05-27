# IM

### 项目说明及目录

**简介**

本课题使用WebSocket和SignalR来实现一个简单的跨平台实时通讯应用。该应用支持用户在Web浏览器或Android App上完成一对一，一对多以及多对多地实时聊天，除了能够发送文本消息外，也可以实现发送图片消息，以及一般二进制文件的传输。

同时课题也实现了一套流式数据传输的演示程序，以模拟生产生活中需要处理流式数据的应用场景，如智慧医疗系统中对患者生命体征数据的监控。 

本课题提供两种实时Web服务器的实现方案。第一种方案基于微软 .NET 5的Web API框架，配合SignalR组件使用C#开发。第二种方案基于Go语言，配合其开源的Web框架Gin和Gorilla/WebSocket组件实现开发。

Web客户端包括Web浏览器和Android平台两种实现。其中Web端使用Vue.JS框架开发，实现了基本的功能演示页面。同时在网络层使用Vuex组件分别实现了针对SignalR服务器和Go服务器（WebSocket）两种通信接口的封装。Android端使用Kotlin语言，配合SignalR组件的Java客户端支持完成开发。

**.NET服务器:**

https://github.com/HaoyuanMa/IM-Api

**Go服务器:**

https://github.com/HaoyuanMa/IM-Api-go

**Web客户端:**

https://github.com/HaoyuanMa/IM-Front-Web

**Android客户端:**
 
https://github.com/HaoyuanMa/IM-Front-Android

**流式数据生成程序:**

https://github.com/HaoyuanMa/IM-DataStreamGenerator-CSharp

https://github.com/HaoyuanMa/IM-DataStreamGenerator-go
