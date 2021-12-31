Docker-compose stand with RabbitMQ and sender/reciever.
---
## About
First app is a producer that sends messages (1 per second / while-true loop), the second one is a consumer that receives messages and prints them out.

## Requirements
* Docker-compose

## How to run
```
git clone https://github.com/7olstoy/go-rabbitmq-docker-sample
cd go-rabbitmq-docker-sample
docker-compose up
```
After, you can check RabbitMQ internal dashboard at ```http://localhost:15672```.

## Version with grafana dashboard and monitoring
```
git clone https://github.com/7olstoy/go-rabbitmq-docker-sample
cd go-rabbitmq-docker-sample
docker-compose -f docker-compose.monitoring.yml up
```
After, you can check Grafana RabbitMQ dashboard at ```http://localhost:3000``` and admin:admin credentials. 

## Links
* Go code from [official](https://www.rabbitmq.com/tutorials/tutorial-one-go.html) rabbitmq docs.
* Grafana dashboards from [official](https://github.com/rabbitmq/rabbitmq-server/tree/master/deps/rabbitmq_prometheus/docker/grafana) rabbitmq repo.
