
Meeting notes for Isabella, Oliver, Joy and me

## 000. Consistent Hashing
**Meeting Date/Time:** 07/25/2021 

**Speaker:** XiuYi 

**Attendees:** Oliver, Isabella, Joy

**Meeting Notes:**

* Scalability
* 服务器的负载均衡算法
* 分布式缓存场景，3万张图片，3个缓存服务器
* 传统Hash取模算法，所有的缓存数据hash值改变，All cache miss
* 一致性hash算法，先hash服务器编号，然后hash文件/请求的名字，只有小部分缓存失效
* 数据倾斜/某台服务器宕机，请求分散
* 代码


## 001. 1) Oliver: 缓存简介，缓存更新策略（上）; 2) Joy：DDIA第一章; 
**Meeting Date/Time:** 07/27/2021 

**Speaker:**  Oliver, Joy

**Attendees:** XiuYi, Isabella

**Meeting Notes:**

Oliver: 缓存简介，缓存更新策略（上）
* [缓存Eviction policies](https://www.educative.io/courses/grokking-the-system-design-interview/3j6NnJrpp5p)
* [缓存失效的更新，Write Through, Write Back, Write Around](https://www.educative.io/courses/grokking-the-system-design-interview/3j6NnJrpp5p)
* [扩展阅读1-Redis小结](https://zhuanlan.zhihu.com/p/59168140)
* [扩展阅读2-双写一致性方案](https://www.cnblogs.com/rjzheng/p/9041659.html)

Joy：DDIA第一章
* Reliability
* Scalability
* Maintainability


## 002. 1) push/pull & Polling; 2) Inverted Index; 
**Meeting Date/Time:** 07/30/2021 

**Speaker:**  Isabella, XiuYi

**Attendees:** Joy, Oliver

**Meeting Notes:**
 
 push/pull & Polling
* short polling/long polling/websocket
* pull/pull各自适用场景

Inverted Index
* 关键词为key，出现地方为value
* lucene，Solr/ElasticSearch

## 003. 1) 如何保证消息的时序性 2) 缓存简介，缓存更新策略（下）
**Meeting Date/Time:** 07/31/2021 

**Speaker:** XiuYi, Oliver

**Attendees:** Isabella, Joy

**Meeting Notes:**

如何保证消息的时序性
* 分布式，集群化部署
* 全局ID generator
* 离线推送

缓存简介，缓存更新策略（下）
* Weak/Eventual/Strong Consistency
* data parition - tweet id
* fail over / replication
* cache aside(write around) / write back / write through / refresh ahead

## 004. 1) API设计要点 2) BQ准备，亚麻16条领导力准则
**Meeting Date/Time:** 08/05/2021 

**Speaker:** Isabella, Xiuyi

**Attendees:** Oliver, Joy

**Meeting Notes:**

API设计要点
* RPC
* SOAP
* REST
* GraphQL

BQ准备，亚麻领导力准则
* 自我介绍
* 1）客户至上； 2） 主人翁精神； 3）创新简化； 4）决策正确

## 005. 1) SDP - Database, RDBMS, NoSQL 2) DDIA第二章
**Meeting Date/Time:** 08/08/2021 

**Speaker:**  Oliver, Joy

**Attendees:** Isabella, Xiuyi

**Meeting Notes:**
1）Oli - SDP - Database
* #1: Relational database management system (RDBMS)
  * master-master, master-slave, federation, sharding
* #2: NoSQL
  * Key-Value Store, Documentation Store, Wide-Column Store, Graph Database  
* #3: SQL or NoSQL
* [SDP](https://github.com/donnemartin/system-design-primer)

2）Joy - DDIA Chapter II 
* SQL/Nosql 
* 关系型 文档型

## 006. 1）Design Chat Service (Grokking) 2）MicroService
**Meeting Date/Time:** 08/12/2021 

**Speaker:** Joy, Isabella

**Attendees:** Oliver, Xiuyi

**Meeting Notes:**
1) Design Chat Service (Grokking)
* polling - WS
* consistency
* store - column based
* partitioning

2）MicroService
* Introduction

## 007. 1)Xiuyi讲Chat Service补漏 2) Oliver分库分表
**Meeting Date/Time:** 08/15/2021  

**Speaker:** Oliver, Xiuyi

**Attendees:** Joy, Isabella

**Meeting Notes:**
1) chat 补充
* polling and websocket
* push vs pull
* 流程图

2) 分库分表
* 策略
* join操作

## 008. 1）Joy讲IG， 2）Xiuyi复习Isabella的topics
**Meeting Date/Time:** 08/19/2021  

**Speaker:** Joy, Xiuyi

**Attendees:** Isabella, Oliver

**Meeting Notes:**
1) 
*
2) 
* 

## 009. 1）Oliver算法模板， 2）Isabella复习Joy的topics
**Meeting Date/Time:** 08/22/2021 

**Speaker:** Oliver， Isabella

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 算法模板
* Binary Search
* Two Pointer
* BFS
* BT/BST
* DP
* Heap
* Union Find
* Trie
2) 
* 

## 010. 1）Joy复习Oliver的topics 2）Xiuyi - Load Balancer
**Meeting Date/Time:** 08/26/2021 

**Speaker:** Joy, Xiuyi

**Attendees:** Oliver， Isabella

**Meeting Notes:**
1) From grokking
* Load Balancer
* caching
* Data Partitioning
* SQL/NoSQL
* CAP
* Long Polling, WB, Server sent events(SSE)

2) 
* Load Balancer必知必会

## 011. 1）Isabella复习Facebook message和IG
**Meeting Date/Time:** 08/29/2021 

**Speaker:**  Isabella, Oliver

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 
* session ID 是否可以用全局ID生成器例如Redis？
* 

## 012. 1）Desgin Youtube 2) pre sum
**Meeting Date/Time:** 09/02/2021 

**Speaker:** Joy，Oliver， 

**Attendees:** Isabella, Xiuyi

**Meeting Notes:**
1) 
* cache storage

2) 
* tech blog

## 013. 1）Notification 2) Job Scheduler
**Meeting Date/Time:** 09/05/2021 

**Speaker:** Xiuyi， Isabella

**Attendees:** Joy, Oliver

**Meeting Notes:**
1) 
*
2) 
* 

## 014. 1）Joy复习Xiuyi的topics 2）多线程
**Meeting Date/Time:** 09/10/2021 

**Speaker:** Joy, Xiuyi

**Attendees:** Oliver， Isabella

**Meeting Notes:**
1) 复习topics
* 一致性hash
* Inverted Index
* Cookie, Session, Token
* Load Balancer
2) 
* 

## 015. 1）Isabella复习Xiuyi的topics 
**Meeting Date/Time:** 09/12/2021 

**Speaker:** Isabella

**Attendees:** Joy, Xiuyi 

**Meeting Notes:**
1) 复习topics
* 
2) 
* Learn and Be Curious
* Earn Trust

## 016. 1）Tiny URL 2）Typeahead
**Meeting Date/Time:** 09/17/2021 

**Speaker:** Joy, Oliver

**Attendees:** Xiuyi, Isabella

**Meeting Notes:**
1) Tiny URL
* 不同短网址在不同网站上，检测访问量
* 一个长网址对应多个短网址(Cassandra等column based)
* 服务器和用户可设置过期时间，不能被猜到
* hash function
* Key generation Service生成短网址的letters， 6个8个等
2) Typeahead
* 

## 017. 1）网络安全基础 2）Design Parking lot
**Meeting Date/Time:** 09/19/2021 

**Speaker:** Xiuyi, Isabella

**Attendees:** Oliver， Joy

**Meeting Notes:**
1) 
* 
2) 
* 

## 018. 1）图论，DP基础 2）Union Find
**Meeting Date/Time:** 09/28/2021 

**Speaker:** Joy, Isabella

**Attendees:** Oliver， Xiuyi

**Meeting Notes:**
1) 图论入门
* Queue
* Priority Queue
2) Union Find
* 

## 019. 1）设计KV Store
**Meeting Date/Time:** 09/30/2021 

**Speaker:**  Xiuyi

**Attendees:** Oliver，Joy, Isabella and many others

**Meeting Notes:**
1) 设计KV Store
* 
* 
2) 
* 

## 020. 1）Grokking新的topics 2）Design Rate Limiter 3)
**Meeting Date/Time:** 08/22/2021 

**Speaker:** Joy, Isabella, Oliver

**Attendees:** Xiu Yi

**Meeting Notes:**
1) 
* Redundancy (server) and Replication(data)
* Bloom Filters - 不为1肯定没有，为1不保证一定有
* Quorum
* Leader and Follower
* Heartbeat
* Checksum - 对TCP/UDP的报文段进行校验/检测nodes之间数据复制是否完整
2) Design Rate Limiter
* Token bucket
* 
3) 
* 

## 021. 1）Isabella复习LB/Consistent Hashing/Partitioning,Sharding 2）Blind 75
**Meeting Date/Time:** 10/07/2021 

**Speaker:**  Isabella, Oliver

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 
* 
* 
2) 
* 


## 022. 1）亚麻领导力LP学习4条
**Meeting Date/Time:** 10/12/2021 

**Speaker:**  Xiuyi 

**Attendees:**  Isabella, Oliver

**Meeting Notes:**
1) 
* Learn and Be Curious 好奇求知
* Hire and Develop The Best 选育贤能
* Insist on the Highest Standards 最高标准
* Think Big 远见卓识


## 023. 1） Design Pastebin 2）复习2
**Meeting Date/Time:** 10/14/2021 

**Speaker:**  Joy，Isabella

**Attendees:** Xiuyi

**Meeting Notes:**
1) 
* paste table + user table
* clean service
2) 
* peer to peer / master slave
* Cahce （缓存淘汰策略，缓存与DB一致性问题 - 先更新DB再删缓存，脏数据最少）

## 024. 1）API的设计 2）读书分享 - Working Effectively with Legacy Coding第一章
**Meeting Date/Time:** 10/19/2021 

**Speaker:**  Xiuyi, Oliver

**Attendees:** Isabella

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 025. 1）Design Dropbox 2）Idempotency幂等
**Meeting Date/Time:** 10/21/2021 

**Speaker:**  Joy, Xiuyi

**Attendees:** Oliver, Isabella

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 026. 1）Review basics III - databases 2）读书分享 - Working Effectively with Legacy Coding第二章
**Meeting Date/Time:** 10/24/2021 

**Speaker:**  Isabella, Oliver

**Attendees:** Joy, Xiuyi

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 027. 1）Mock Job Scheduler 2）Distirbuted Lock
**Meeting Date/Time:** 10/31/2021 

**Speaker:**  Isabella, Xiuyi

**Attendees:** 

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 028. 1）设计Twitter的补充 2）TopK的设计 3) Multi-threading
**Meeting Date/Time:** 11/07/2021 

**Speaker:**  Joy, Isabella, Xiuyi

**Attendees:** 

**Meeting Notes:**
1) 
* tweets的Sharding - 雪花算法ID
* Cache
* Twitter Search
2) 
* MapReduce
* Count-min Setch
3) 
* 可重入性的问题

## 029. 1）Mock Interview设计Amazon Price Tracker
**Meeting Date/Time:** 11/14/2021 

**Speaker:**  Xiuyi

**Attendees:** Isabella, Joy, Oliver

**Meeting Notes:**
1) 
Amazon price tracker

1k products

requirements: 

1) grab the prices and store prices somewhere

2) we pop these date to customers

Amazon prices -> services to grab the prices -> to our own stores - > services to fetch data from our stores -> pop up for 
ASAP for real time for customer needs

1) pay Amazon to use APIs to get data - alternative for others, we may can use crawlers

2) rest/graphQL APIs to get data in our gateway layers - json objects

3) middle ware service to clean/aggregate/cluster data - pre-compute

4) store

shcema:

	Product: productID, categoryID, price, timestamp;
	
	Price: ID, productID, Array{{price1, time1},{price2, time2},{price3, time3}...}
	
	Category: ID, categoryNames....
	
```sql
Select price From Product Where ProductID = "123" 
```

5) sevices to grab data and do some computing - pick some products/category,save them in the cache -> speed reading for new customers

6) pop to clients

authozation -> free -> can access some limited resources (e.g, overal category prices change in past three months) vs VIP users (have more accesses to all tracks, like all historical data changes for all produces)

![架构图](/meetingPPT/imgs/029Arch.png)

## 030. 1）点赞系统 2）Kafka入门图解
**Meeting Date/Time:** 11/18/2021 

**Speaker:**  Isabella, Xiuyi

**Attendees:** Joy, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
* kafka不在一个consumer group的消费者怎么消费同一个消息？

## 031. 1）Design slack - 0
**Meeting Date/Time:** 12/02/2021 

**Speaker:**  Xiuyi

**Attendees:** Isabella, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
* 

## 032. 1）Neayby Friend; 2) 点赞系统 - 续 3) Manage up
**Meeting Date/Time:** 12/05/2021 

**Speaker:**  Joy, Isabella, Xiuyi

**Attendees:** Oliver

**Meeting Notes:**
1) 
* Quad Tree
* 
2) 
*
3)
*

## 033. 1）[Counting system](https://medium.com/pinterest-engineering/building-a-real-time-user-action-counting-system-for-ads-88a60d9c9a
); 2) GeoHash 
**Meeting Date/Time:** 12/05/2021 

**Speaker:**  Isabella, Xiuyi

**Attendees:** Joy, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)
*

## 034. 1）Partition之前的一些策略; 2) Design Snapchat/instagram Stories 3) DDIA summary - ch 1,2
**Meeting Date/Time:** 12/05/2021 

**Speaker:**  Joy, Isabella, Xiuyi

**Attendees:** Jasmine

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)
*

## 035. 1）Design What's up app 2) Distributed System Summary + k8s
**Meeting Date/Time:** 01/02/2022

**Speaker:**   Isabella, Xiuyi

**Attendees:** 

**Meeting Notes:**
1) 
* 
* 
2) 
*

## 036. 1）Design What's up app - leftover 2) DDIA ch 3
**Meeting Date/Time:** 01/09/2022

**Speaker:**   Isabella, Xiuyi

**Attendees:** Joy, Oliver, Jasmine

**Meeting Notes:**
1) 
* 
* 
2) 
*

## 037. 1）DDIA ch 4 2) In Memory DB 3) Design Leetcode
**Meeting Date/Time:** 01/16/2022

**Speaker:** Xiuyi, Nick, Isabella

**Attendees:** Joy

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)


## 038. 1）Twitter Architecture
**Meeting Date/Time:** 01/23/2022

**Speaker:** Xiuyi

**Attendees:** Jasmine, Nick, Isabella, Oliver

**Meeting Notes:**
1) 
* 
* 
2) 
*
3)


## 039. 1）Zero Copy 2) Apache Flink 3) Cost Efficiency @ Scale in Big data File Format
**Meeting Date/Time:** 01/23/2022

**Speaker:** Xiuyi, Isabella, Oli

**Attendees:** Jasmine, Nick, Joy

**Meeting Notes:**
1) 
* 
* 
2) 
* https://developer.aliyun.com/article/666052?spm=a2c6h.13262185.0.0.4c7b7e18EzjqIJ

3)
* https://eng.uber.com/cost-efficiency-big-data/

