## Kafka

producer
|
(TCP)
|
broker (9092)
[topic, partitions, Zookeeper]
|
(?)
|
consumer
(each psrtition has to be consumed by only 1 consumer group)

consumer(one) ->(to) producer(many)

pub sub model, write once read multiple

to act like a queue, put everything in one partition

ZooKeeper
leader, follower concept
[broker]
(multiple nodes to ensure modularity)

only leader can be written to
