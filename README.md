# Questions
## Amount of data sent to the message broker in one run
The amount of data is equivalent to the amount of `publish_event`, which is 5.

## `amqp://guest:guest@localhost:5672`
It is the same as in **subscriber** because it is sending to the same host with the same port with the same credential.

# Screenshots
RabbitMQ
![Alt text](image.png)

## What happened?
When subscriber and publisher is run, subscriber will receive five messages from publisher.
![Alt text](image-1.png)

## Spike and Publisher
The spike is representing the consumer ack count within that period. Consumer ack refers to the acknowledgement sent by consumer to the RabbitMQ broker to confirm that a message has been successfully received and processed.

![Alt text](image-2.png)