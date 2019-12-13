## 环境搭建

+ python3.5+
+ RabbitMQ
+ Redis 3.2.1
+ Nameko 2.11.0
+ Swagger
+ Flask 1.0.2


## RabbitMQ docker 安装命令
```shell
docker search rabbitmq
docker pull rabbitmq
docker run -d --hostname my-rabbit --name some-rabbit -p 15672:15672 -p 5672:5672 rabbitmq
```


## 运行

```shell
git clone
cd microservices
nameko run push & nameko run register
cd .. & python app/api.py
```


访问:http://localhost:5000/apidocs/#/