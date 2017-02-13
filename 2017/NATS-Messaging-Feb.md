#Briefing Notes: NATS.io

[NATS](http://nats.io) is a modern messaging platform focussed on cloud native applications, with an unique advantage for Microservices architectures. In this briefing note, we take a look at NATS platform, comparing it with both legacy and other modern messaging platforms, and do a SWOT analysis to our clients considering the platform for their use.

##Market Overview

Modern messaging platforms emerged from the messaging middleware of the past and it is gaining more importance with distributed infrastructure and microservices based application architectures. Traditional middleware messaging platforms focussed on more enterprise features, like delivery guarantees, than what is needed for microservices architectures. However, there are use cases where some of these traditional platforms are applicable but modern messaging platforms focus more on being lightweight and on features like developer experience, RESTful interface, scalability, etc..They are built much in tune with the underlying modern distributed infrastructure like cloud platforms.

##NATS Messaging Platform

NATS is an open source messaging system by Apcera focussed on being lightweight with RESTful interface, highly scalability and better performance. The core server is written in Golang with clients in more than a dozen languages including Python, Ruby, Node.js, Elixir, Java, C and C# (This list includes third party contributions). They also have libraries available in various languages. The supported use cases include distributed queueing, pub/sub, Request/Response and they recently announced support for realtime streaming.

##SWOT Analysis

###Strengths
* Lightweight and RESTful, suitable for IoT and Microservices
* Client and libraries available in many languages
* Proven scalability and low resource usage. Public case studies available from users talking about how they are using NATS with 10 Million + concurrent connections with better resource utilization
* Better developer experience, making it attractive for developers wanting to build scalable microservices

###Weakness
* Lack of backend support from modern platforms. Right now Apcera, Pivotal CloudFoundry (experimental support) and few other smaller/niche platforms support this as a messaging layer and there are third party OSS connectors for many other platforms like Kubernetes, Docker, Rancher, etc.. However, having support from platform vendors is needed for wide enterprise adoption
* Not many enterprise focussed features or support for SLAs, making NATS a good platform for only cloud native, IoT and Microservices. This is not really a weakness in the Modern Enterprise context but enterprises having investments in other messaging platforms may not want to use a different platform for modern apps. However, they are working on clustering support for NATS which should make the platform more attractive for enterprises with failover and HA

###Opportunities
* Being a Lightweight RESTful platform and having a good traction for IoT and Microservices use cases may help NATS emerge as the defacto standard for these use cases
* Since NATS is open source, it gives an opportunity to extend the platform capabilities and reach more easily than a proprietary platform

###Threats
* NATS, at this moment, is a single vendor backed OSS project with few contributors in Github. It is important for them to expand and diversify the contributors. They are in the process of streamlining the contribution process and building up documentation for developers
* Lack of a business model around NATS is definitely a threat. The team understands the need and they are exploring various options. Monetizing OSS is difficult but the fact that they have an enterprise grade platform (Apcera) will help them explore interesting opportunities

##Conclusion

NATS is a robust and lightweight messaging platform widely preferred by developers for Cloud Native, IoT and Microservices use cases due to high scalability and better performance. If they add more and diverse set of contributors and add support for more container based platforms, they could emerge as the go to messaging platform for the use cases mentioned above. One way to build a strong community is by making this project a part of Cloud Native Computing Foundation or one of the larger OSS foundations.

##Competitors

Redis Pub/Sub, ZeroMQ, RabbitMQ, ActiveMQ, Apache Kafka, Tibco EMS
