## Spring Boot WebSocket Chat Appplication

You can checkout the live version of the application at https://spring-ws-chat.herokuapp.com/

![App Screenshot](screenshot.png)

## Requirements

1. Java - 11

2. Maven - 3.x.x

## Steps to Setup

**1. Clone the application**

```bash
git clone https://github.com/callicoder/spring-boot-websocket-chat-demo.git
```

**2. Build and run the app using maven**

```bash
cd spring-boot-websocket-chat-demo
mvn package
java -jar target/websocket-demo-0.0.1-SNAPSHOT.jar
```

Alternatively, you can run the app directly without packaging it like so -

```bash
mvn spring-boot:run
```

## Learn More

You can find the tutorial for this application on my blog -

https://www.callicoder.com/spring-boot-websocket-chat-example/

##  Docs
- https://blog.scaleway.com/iot-hub-what-use-case-for-websockets/
- https://medium.com/ballerina-techblog/go-real-time-with-ballerina-websockets-58c40ac11d6
- https://www.educba.com/mqtt-vs-websocket/

## Uses Cases
For those reading of you who simply want to know if you should choose WebSockets or REST for your next project, here’s a simple rule: if any of the following sounds like your application, then use WebSockets. If not, stick to traditional HTTP/REST requests:

* Real-time collaboration (Google Docs, Easybase)
* Social feeds (Twitter, Discord)
* Image/text chat (Messenger, Snapchat)
* Synchronizing across multiple sessions (Todoist, Dropbox)
* News/score updates (ESPN, CBS Sports)
* Multiplayer game (Lichess)

