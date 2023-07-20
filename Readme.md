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

## STOMP 

STOMP which stands for Simple Text Oriented Messaging Protocol is a sub protocol which runs on top of Websocket connections and is used for message exchanges between clients via an intermediate message broker.

STOMP has client implementations in different languages such as in Javascript(stomp-js) and Java, to interact with a Springboot Server over websockets. Do go through this amazing article to understand how Springboot over websockets with STOMP works.

Now let us go over building a python client with the required springboot server configurations for interactions between the two.

* https://srinivas1996kumar.medium.com/a-python-stomp-client-for-interaction-with-a-springboot-server-6acc00b90014

  ![IOT  RabbitMQ Stomp](https://github.com/sanogotech/spring-boot-websocket-chat-demo/blob/master/divers/rabbitStompWebJsIOT.png)



# RabbitMQ docker image with STOMP plugin enable

[![ci](https://github.com/quangthe/docker-rabbitmq-stomp/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/quangthe/docker-rabbitmq-stomp/actions/workflows/docker-publish.yml)
[![Docker Stars](https://img.shields.io/docker/stars/pcloud/rabbitmq-stomp.svg?style=flat)](https://hub.docker.com/r/pcloud/rabbitmq-stomp/)
[![Docker Pulls](https://img.shields.io/docker/pulls/pcloud/rabbitmq-stomp.svg?style=flat)](https://hub.docker.com/r/pcloud/rabbitmq-stomp/)

Check image tags on [DockerHub](https://hub.docker.com/repository/docker/pcloud/rabbitmq-stomp/tags)

## Quick start

```
docker pull pcloud/rabbitmq-stomp

docker container run -it --name rabbitmq-stomp -p 15672:15672 -p 5672:5672 -p 61613:61613 pcloud/rabbitmq-stomp
```

- RabbitMQ Web UI: [localhost:15672](http://localhost:15672)
- Credential RabbitMQ: `admin/admin`
- Credential STOMP: `admin/admin`




### Exposed ports

- `5672`: Default port of RabbitMQ
- `15672`: RabbitMQ Web UI
- `61613`: STOMP port
