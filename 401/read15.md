# Event Driven Architecture

**What’s the difference between a FIFO and a standard queue?**
FIFO queues provide exactly-once processing, which means that each message is delivered once and remains available until a consumer processes it and deletes it.

**How can the server be assured a message was properly received?**
 The messages sent by the client, usually a Web browser, are called requests ... Each individual request is sent to a server,

**What classic design pattern is best represented by event driven programming?**

When talking about Event-Driven Systems, this distinction helps vocalizing the intent behind sending a message.

**How do you test an event driven system?**
the Order Service acts as an orchestrator, coordinating actions of all the other services, typically through a direct API call. This service is the brains of the system and is responsible for enforcing business rules around the order lifecycle, such as sending an email notification to the customer, when the order has been shipped.


# Term


**FIFO Queue**:
FIFO (First-In-First-Out) queues are designed to enhance messaging between applications when the order of operations and events is critical, or where duplicates can't be tolerated.

**Pub/Sub**:
Pub/Sub allows services to communicate asynchronously, with latencies on the order of 100 milliseconds.



# Preview


**Which 3 things had you heard about previously and now have better clarity on?**
all thing 
**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**
all thing also , it's hard 

**What are you most excited about trying to implement or see how it works?**
understand the socket 




# SNS is a distributed publish-subscribe system. Messages are pushed to subscribers as and when they are sent by publishers to SNS.

**SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll or pull messages from SQS. Messages can't be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later. Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers. SNS supports several end points such as email, SMS, HTTP end point and SQS. If you want unknown number and type of subscribers to receive messages, you need SNS.*




**The AWS Lambda service internally uses the continuous long-polling technique to fetch messages from the SQS queue. This counts against the API requests, so your account will be charged for those API calls. So even if your SQS queue is empty for days, you may still see API usage in your detailed bill report.**


