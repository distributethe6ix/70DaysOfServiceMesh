## 7 - Resilient Microservices
> **Tutorial**
>> *Let's build some resilient microservices*

### What is resiliency in this context?
Imagine going to the bank and waiting in line to see a teller. The queue is so long, and it's taking roughly 15 minutes per person to be seen and there are 6 ahead of you. Only 2 tellers are seeing folks. So anywhere from 45-60 minutes you'll be seen. After a while some folks decide to leave the line, but then you notice it's because one teller left. Now there are 4 ahead of you but one teller. You're getting quite nervous, because you have a meeting. Finally, you're next in line, but you're meeting starts in 15 minutes and you need time to drive home, so you decide to just leave. 

With microservices, it's highly unpredictable to determine the network conditions can change, and a resource can suddenly become unavailable. Service Mesh solves this problem by implementing structure, timing, and conditions around what needs to happen when "x,y and z" occur. This is so requests can be navigated through these ever-changing conditions and be provided with actual or meaningful responses. A more clearer example is how services call each other and how long they have to wait. Some services could be left waiting for a while, because the upstream service is waiting for a response. This has a cascading effect on the overall round-trip-time of that response. This adds latency. 

There are mechanisms that can be deployed like retires, timeouts, circuit break and fault injection

Also, something needs to implement this, and in the case of Istio, it's the sidecar.

#### Timeouts
A timeout is used to effectively force a decision on when to give up on that request to a service. If it responds within the timeout window, great, but if it hits the limit, the request is terminated.

#### Retries
Retries allow for a requests to be retried if a request fails. The sidecar will be responsible for implementing the retry call to the failed service. 

#### Circuit Breaking
Circuit breaking offers yet another mechanism to build resiliency into an application. Thresholds can be set to prevent a service from being overloaded. For example, 

#### Fault Injection

Istio offers a great deal of capabilities around building resiliency 