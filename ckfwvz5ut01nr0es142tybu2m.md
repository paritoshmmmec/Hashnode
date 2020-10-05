## Tail latency

### What is tail latency?

Tail latency is the small percentage of response times from a system, out of all of the responses to the input/output (I/O) requests it serves, that takes the longest in comparison to the majority of its response times. (jiber jabber)

In a nutshell, if you are developing a system and let us say you are serving 1000 users and if you have a latency of all 1000 users (sorted by time) then whatever comes at 990 indexes is the value of how you are serving 99 percentile of users aka(p99 percentile of users).


### Why tail latency?

Things don't go smoothly as we think during development. 
Networks can go flaky, disk reads can be slow or database is under heavy load. So If your p99 latency is higher, it means one customer can suffer a lot which can result in losing business.


In summary, tail latency is good metrics as it correlates directly to business health so the first step is to start measuring it. 