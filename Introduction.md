Introduction to Redis
## Redis介绍
Redis is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker.   
---
redis是一个开源（BSD licensed 协议）的内存数据结构存储，一般用作数据库、缓存和消息代理。
---
It supports data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, geospatial indexes with radius queries and streams.   
---
它支持的数据结构有：Strings、hashes、lists、sets、范围查询的有序Sets、bitmaps、hyperloglogs、geospatial indexes with radius queries and streams。
---
Redis has built-in replication, Lua scripting, LRU eviction, transactions and different levels of on-disk persistence, and provides high availability via Redis Sentinel and automatic partitioning with Redis Cluster.
---
redis内置了复制、lua脚本、LRU驱动事件、事务和不同级别的磁盘持久性，并且通过redis哨兵和Redis集群的自动分区实现高可用。
---
You can run atomic operations on these types, like appending to a string; incrementing the value in a hash; pushing an element to a list; computing set intersection, union and difference; or getting the member with highest ranking in a sorted set.
---  
你可以在这些类型上执行原子操作，比如追加到字符串；递增哈希值；压入一个元素到list；计算set的交集、并集和差集；或者在有序集合中获得排名最高的元素。
---
In order to achieve its outstanding performance, Redis works with an in-memory dataset. Depending on your use case, you can persist it either by dumping the dataset to disk every once in a while, or by appending each command to a log. Persistence can be optionally disabled, if you just need a feature-rich, networked, in-memory cache.

---
为了实现它杰出的性能，Redis使用内存数据集。根据你的使用场景，你可以每隔一段时间转存数据集到硬盘中，也可以使用追加操作日志的方式去持久化数据。如果你仅仅需要功能丰富的网络内存缓存，可以选择关闭数据持久化。
---
Redis also supports trivial-to-setup master-slave asynchronous replication, with very fast non-blocking first synchronization, auto-reconnection with partial resynchronization on net split.
---
Redis也支持主从异步复制的配置，具有非常快速的非阻塞第一次同步，自动重新连接以及在网络分割上的部分重新同步。
