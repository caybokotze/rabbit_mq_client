# Rabbit MQ - A basic consumer and producer.

This is a simple illustration of how to use the RabbitMq message service to send and receive message through the queue using asp.net core 3.1.

## Why use Rabbit Mq?

Rabbit Mq is a open source messaging platform that allows your applications / services to communicate with each other very rapidly. The advantage being you can run processes in parallel and set up many worker services to respond to the same or various different service calls.

## What are the alternatives?

- [ ] You could consider using Redis cache for applications where you need to store a lot of information in RAM.
- [ ] Eclipse Mosquitto is a good option to consider as a open source message broker over the Mqtt protocol.
- [ ] Apache Kafka is also a good option to look at although it might be overkill for a lot of applications. 
- [ ] HiveMq is also a good messaging broker for clustered messaging brokers that need to handle millions of messages per second. Do keep in mind the free version only allows for 25 service connections to one broker.

There are a few other messaging services available ont he web. Ultimately it depends what you are building your solution for. Some are better for different use cases. So it is up to you.

## Requirements to get started.

- [ ] Install Dotnet Core SDK. <a href="https://dotnet.microsoft.com/download" target="_blank">Click here.</a>
- [ ] Install Erlang first. <a href="https://www.erlang.org/downloads" target="_blank">Click here.</a>
- [ ] Install RabbitMq. <a href="https://www.rabbitmq.com/download.html" target="_blank">Click here.</a>

### What is a producer?

A producer is a the way Rabbit Mq defines a service that publishes messages onto a message bus / queue.

### What is a consumer?

A consumer is how RabbitMq defines a service that receives the messages that are being published onto the queue / message bus.

### What is a channel?

A channel is like a topic onto which the producer and consumer subscribe to in order to exchange information. You can set up more than one single channel. Channels / Topics are idempotent so if you create one with the same name twice only one is created.



