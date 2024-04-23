Notice that publisher program will send 5 data to the message broker. This is because the publish event is called 5 times on `main.rs`.

Notice that `amqp://guest:guest@localhost:5672` exists on Subscriber and Publisher. The username and password, server name, and port is the same. This means that both are connecting to the same message broker.

![RabbitMQ Screenshot](RabbitMQ.png "RabbitMQ")

![RabbitMQ Screenshot](RabbitMQ_Connection.png "RabbitMQ")

![RabbitMQ Screenshot](TerminalSubscriber.png "RabbitMQ")

![RabbitMQ Screenshot](TerminalPublisherpng.png "RabbitMQ")

Here, we tried to send information using Publisher. Everytime we hit `cargo run` on publisher, the spike get up.

![RabbitMQ Screenshot](RabbitMQ_Connection_2Spike.png "RabbitMQ")

Monitoring chart based on publisher. On this screenshot, we tried to make 2 spikes. I tried to hit publisher lots of times on 2 periods. This is to mae those two spiker
