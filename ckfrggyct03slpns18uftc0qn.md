## Reasons to (not) adopt Kafka

### Why I am writing this

I am trying to write this article to put some** food for thought * for you before adopting Kafka. As a developer, we should always be careful when adopting any technology, as it may cost you a lot down the road. This might also put some rationale if you trying to convince the team member to choose Kafka over other solutions. 

Bonus: Read this article about  [Magpie bird
](https://blog.codinghorror.com/the-magpie-developer/)  haha

### Introduction

Message brokers are not a new concept. However, technologies have been matured a lot in the last decade or so.  Since the inception of Kafka, it is certainly been an innovative community [here].


### Reason to Adopt Kafka

1. **High rate of ingestion**:   If your app has to accept a large number of messages/events, Kafka is certainly a better choice. All you need to add more brokers and partitions. 

2. **Central hub for data**:  If you want to build a central platform that can feed data to BI platforms or data lake systems or analytics platforms, Kafka is your friend. 

3. **Connector for different ecosystems **:  This is one of the biggest advantages of the Kafka, as a large community is involved to deliver the innovative solutions and have delivered 100 of connector b/w different ecosystem. e.g. you can send data from SQL server to salesforce or vice versa. This kind of integration puts Kafka on the drive. 

4. **History of messages **: If you have to read the message from the past, this solution is only available in Kafka and Pulsar. Pulsar also supports tiered storage so you can save data for ages (I am not kidding).

5. **Inexpensive infrastructure cost **:  As Kafka writes messages in sequence, so you can real performance from sequential writes. So if your company is asking to justify the cost, here you go. 

6. **Unbounded real-time analysis **:  This is one of the best features of the Kafka. This is called streaming where data is coming continuously and you have to detect and act in real-time. This serves various real-world problems e.g. fraud detection, DevOps metrics, location tracking, sensor-based app, and a lot of problems.

7. ** Multiple teams are dependent upon your data **: In a large enterprise, teams are created based on the business area. So you have to create a boundary b/w business entity to separate problems to domain owners. To enable collaboration b/w teams you might need to share some data, Kafka is certainly a better choice. [hint: This is what people call microservices :]

### Reason not to Adopt Kafka

1. ** Need some orchestration b/w message **:   Kafka is written thinking "dumb broker, smart endpoints " so it won't do anything for you.  So if you are looking for ESB kind of solution, Kafka is not a fit.

2. ** Complex coding and configuration **:   Kafka consumer can be very complex to write very soon. Although people are trying to solve to reduce the boilerplate, still a long way to go.

3. ** Default config can be problematic **: Default configs of Kafka can be dangerous so please read all nitty-gritty details e.g. auto committing the message. If on, the message will be lost if the consumer dies without processing the message. This is not good if you cannot afford to lose the message. [Although a distributed system can lose message anytime]

4. ** Confluent drive the Kafka ecosystem **: Companies are notorious for there profit-margin stuff. Although Confluent is the driving force behind Kafka's growth, it is a risk too.  


There you go, play around with Kafka and share your experience.

See ya later





