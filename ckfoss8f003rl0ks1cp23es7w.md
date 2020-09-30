## Kafka key concepts

In recent years, Apache Kafka has become a de-facto technology raging from solving central hub for data exchange b/w services or streaming data in real-time to detect frauds. Here directly from the Kafka web-site: 

> 
Kafka is a distributed system consisting of servers and clients that communicate via a high-performance TCP network protocol. It can be deployed on bare-metal hardware, virtual machines, and containers in on-premise as well as cloud environments.


## Key Concepts

###  Topic

Imagine it like a music folder where you store files underneath.
If you want to listen to music, you can open the whole folder in a music player (consumer) it can run one by one. Doing so you can look at all the data under one label `music`. Similarly in Kafka, data or message go under a single label called a topic. so in nutshell:


> 
A Topic is a category/feed name or logical concept to which records are stored and published. All Kafka records are organized into topics. 

### Brokers

You can imagine brokers like the OS of the computer which does all the stuff e.g. if you are copying some data from one location to another location, you issue a command to os which does the real transfer of data and makes sure the integrity of data.

In the Kafka world, this is called brokers which sits b/w Kafka ecosystem and underlying storage technology. You can a single broker for the cluster but that can fail any time. All Kafka cluster has a primary broker (like mom or your sibling at home) which handles all the stuff along with backup broker (e.g. you or your father) which can serve as a backup in case the primary backup is not working up to date. Having multiple brokers in the Kafka cluster is a good practice.

### Partitions

To continue on the above analogy, Imagine If you have one single drive to store all music you ever have and you want to open two different media players (consumers) at the same time. It might not work as expected. In order to solve the problem, you can create two different folders under the music folder where each media player (consumer) from each subfolder independently. This kind of stuff can scale very well in real life. 

This is one of the key features of Kafka do very well. You can create multiple partitions of Topic and thus allow multiple consumers to read at scale. Combining with this, now topics and consumer Kafka can scale infinitely.

### Replications

If you have the only copy of the best opera music, you don't want to lose it. To solve this problem, you create multiple backup copies that will be stored at different locations. This technique called replication. 

In a distributed system, things can go haywire very often e.g. corrupt storage system or network is down.

To solve the disk corruption problem Kafka adopted the replication model. It creates copies of data and store in different partition. 

Let us say you have created a topic with 3 partitions and 2 replications. it will store each incoming message at 2 more places to ensure the safety of data. This feature adds lots of resiliency in your application design as you have reduced the loss of message. 


I will be writing more about Kafka in the future too. Stay tuned.

Please do leave feedback. All comments are welcome. 
