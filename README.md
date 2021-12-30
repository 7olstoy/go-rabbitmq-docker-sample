Go apps with RabbitMQ sample in docker-compose.

# About
Two small dockerized apps in Go and message broker RabbitMQ.
First app is a producer that sends messages (1 per second / while-true loop), the second one is a consumer that receives messages and prints them out.

---
# Requirements
* Docker-compose

# How to run
```
git clone https://github.com/7olstoy/go-rabbitmq-docker-sample
cd go-rabbitmq-docker-sample
docker-compose up
```
After, you can check RabbitMQ dashboard at ```http://localhost:15672```.

# Links
Go code used from [official](https://www.rabbitmq.com/tutorials/tutorial-one-go.html) rabbitmq docs.