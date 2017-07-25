# WebSocket chat sample using Action Cable

This repository is a chat application sample using Ruby on Rails 5 Action Cable.A single Action Cable server can handle multiple connection instances. It has one connection instance per WebSocket connection.


## 1. How to Build Docker Images

### 1.1: build base image
At a command prompt on your host, type the following command:

```
$ docker build -t ror-base -f Dockerfile.base .
```
You can build base image using Ruby on Rails.

### 1.2 build appplication daploy image  
At a command prompt on your host, type the following command:

```
$ docker build -t action-chat -f Dockerfile.onbuild .
```
You can deploy the application using Docker ONBILD.

## 2. How to Run Container
At a command prompt on docker host, type the following command:

```
$ docker run -it --rm -p 3000:3000 action-chat
```

Copy/paste this URL into your browser when you connect

http://<docker-host>:3000/chat_messages/index

I tested it with Google Cloud Platform/Compute Engine.


## Ruby version
>ruby 2.3.3p222
 (2016-11-21 revision 56859) [x86_64-linux]
