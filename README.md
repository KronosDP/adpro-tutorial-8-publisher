Notice that publisher program will send 5 data to the message broker. This is because the publish event is called 5 times on `main.rs`.

Notice that `amqp://guest:guest@localhost:5672` exists on Subscriber and Publisher. The username and password, server name, and port is the same. This means that both are connecting to the same message broker.

RabbitMQ Screenshot

![RabbitMQ Screenshot](RabbitMQ.png "RabbitMQ")
