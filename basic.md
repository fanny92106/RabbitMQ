# RabbitMQ

1. Basic
        
        - RabbitMQ 消息传递稳定性高, 可靠性高
        - MQ 解耦了消息生产者和消息消费者
        - 支持AMQP协议(advanced message queuing protocol, an application layer protocol focusing on process-to-process communication across IP networks)
        - AMQP is a compact protocol(binary protocol), everything sent over AMQP is binary data
    
2. AMQ Model

![AdvancedMessageQueueModel](image/AdvancedMessageQueueModel.png)


3. Models

        1). Basic (Point-to-Point)
        
![ModelPointToPoint](image/ModelPointToPoint.png)

![ProducerBasic](image/ProducerBasic.png)

![ConsumerBasic](image/ConsumerBasic.png)
    
    
      2). Work Queue (Task Queue)
            - 默认使用round-robin轮询机制派发消息给不同的消费者
            - 可以手动设置按劳分配多劳多得机制, 以提高系统效率

![ModelWorkQueue](image/ModelWorkQueue.png)

![ConsumerWorkQueue](image/ConsumerWorkQueue.png)
