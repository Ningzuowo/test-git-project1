[toc]

## NoSQL

![image-20240901232346248](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240901232346248.png)



## Redis

![image-20240901232852852](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240901232852852.png)

![image-20240902144701574](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902144701574.png)

### 通用命令

![image-20240902144715149](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902144715149.png)

### String类型

![image-20240902145340644](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902145340644.png)![image-20240902145352905](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902145352905.png)![image-20240902152727150](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902152727150.png)



### Hash类型

![image-20240902162150738](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902162150738.png)![image-20240902162758402](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902162758402.png)



### List类型

![image-20240902162843512](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902162843512.png)![image-20240902162945697](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902162945697.png)



### Set结构

![image-20240902164542703](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902164542703.png)![image-20240902164820453](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902164820453.png)



### SortedSet

![image-20240902170459829](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902170459829.png)![image-20240902170519495](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902170519495.png)



## Java客户端

![image-20240902171502940](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902171502940.png)

### Jedis

![image-20240902195332136](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902195332136.png)![image-20240902200020466](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902200020466.png)



### Spring Data Redis

![image-20240902200308791](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902200308791.png)

![image-20240902201528114](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902201528114.png)![image-20240902214601031](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902214601031.png)![image-20240902215017439](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902215017439.png)

![image-20240902215930021](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240902215930021.png)![image-20240903104759448](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240903104759448.png)![image-20240903105119916](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240903105119916.png)

![image-20240903105128300](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240903105128300.png)

![image-20240903105600828](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240903105600828.png)



# redis替代session

session生产sessionID返回给浏览器的cookie中，

threadlocal（线程域对象）保存在线程内部，互不干扰

![image-20250219110901080](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250219110901080.png)



负载均衡下，多台tomcat没有相同的session

![image-20250219110026863](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250219110026863.png)

![image-20250219110124851](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250219110124851.png)



![image-20250228130951262](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250228130951262.png)

# 缓存

![image-20240906201101351](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240906201101351.png)

## 缓存更新策略

![image-20240907144103263](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907144103263.png)

![image-20240907144249681](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907144249681.png)

![image-20240907144658921](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907144658921.png)

**先操作数据库，再删除缓存 被穿插的概率低**

![image-20240907145223338](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907145223338.png)

## 缓存穿透

![image-20240907150133032](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907150133032.png)![image-20240907150433778](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907150433778.png)

## 缓存雪崩

![image-20240907150833190](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907150833190.png)



## 缓存击穿

![image-20240907151151961](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907151151961.png)

![image-20240907151539182](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907151539182.png)

![image-20240907151621397](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907151621397.png)

![image-20240907152141970](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907152141970.png)

## 缓存工具封装

![image-20240907154342817](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907154342817.png)

![image-20240907154645010](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907154645010.png)

![image-20240907155035848](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907155035848.png)![image-20240907155106167](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907155106167.png)



# Redis实现全局唯一ID

![image-20240907160120059](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907160120059.png)![image-20240907160359141](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907160359141.png)![image-20240907161430757](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907161430757.png)

# 抢单超卖问题

 ![image-20240907162749830](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907162749830.png)

![image-20240907163026063](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907163026063.png)

![image-20240907163148551](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907163148551.png)

**库存代替版本号**

## 一人一单问题

**事务结束释放锁**

![image-20240907164343900](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907164343900.png)

### 集群模式下仍然存在一人一单安全问题

![image-20240907165042389](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907165042389.png)



# 分布式锁

![image-20240907174422727](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907174422727.png)

![image-20240907174810646](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907174810646.png)

![image-20240907204454465](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240907204454465.png)

## 分布式锁误删问题

![image-20240908151406980](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908151406980.png)

**解决： 给锁加上标识，释放锁时进行锁的标识识别**

![image-20240908151649634](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908151649634.png)

## 判断标识之后，释放锁之前阻塞，锁超时释放

![image-20240908152114434](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908152114434.png)

**保证标识与释放锁的原子性**



## lua脚本

![image-20240908152508950](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908152508950.png)

![image-20240908153511942](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908153511942.png)

![image-20240908154052940](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908154052940.png)

## 总结

![image-20240908155004070](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908155004070.png)



# Redisson



![image-20240908155249269](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908155249269.png)

![image-20240908155434064](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908155434064.png)

## 入门

![image-20240908155558772](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908155558772.png)![image-20240908155616485](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908155616485.png)

## 重入原理

![image-20240908160710737](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240908160710737.png)

![image-20240909091708532](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909091708532.png)

![image-20240909091910594](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909091910594.png)

## 主从一致性问题（联锁：multiLock）

![image-20240909092252215](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909092252215.png)

![image-20240909092457422](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909092457422.png)



# 锁总结

![image-20240909093147609](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909093147609.png)

# 秒杀优化

## 阻塞队列

![image-20240909134331013](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909134331013.png)

![image-20240909135648999](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909135648999.png)

## 消息队列

![image-20240909140250052](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909140250052.png)![image-20240909140354805](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909140354805.png)

### 基于List结构

![image-20240909140517179](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909140517179.png)

![image-20240909140657760](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909140657760.png)

### 基于PubSub

![image-20240909141052596](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909141052596.png)

![image-20240909141118182](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909141118182.png)

### 基于Stream

![image-20240909141602611](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909141602611.png)

![image-20240909141756437](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909141756437.png)

![image-20240909150136122](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909150136122.png)

#### 基于Stream的漏读问题/Consumer Group（消费者组）

![image-20240909150438629](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909150438629.png)

![image-20240909150625277](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909150625277.png)

![image-20240909150858322](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20240909150858322.png)



# 分布式缓存

## 持久化

### RDB

![image-20250208152025091](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208152025091.png)![image-20250208152846371](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208152846371.png)

![image-20250208153000570](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208153000570.png)

### AOF

![image-20250208153247838](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208153247838.png)

![image-20250208153713623](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208153713623.png)

![image-20250208153925206](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208153925206.png)



## Redis主从

### 主从架构

#### 建立主从

![image-20250208154642830](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208154642830.png)

#### 数据同步

##### 全量同步

![image-20250208155108469](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208155108469.png)

![image-20250208155355127](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208155355127.png)

![image-20250208155548795](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208155548795.png)

##### 增量同步

![image-20250208155845917](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208155845917.png)

### 主从优化

![image-20250208230247910](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208230247910.png)



## Redis哨兵

![image-20250208230541593](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208230541593.png)

### 服务状态监控

![image-20250208230644500](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208230644500.png)

### 选取新的（offset）

![image-20250208230801967](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208230801967.png)

### 故障转移

![image-20250208230932018](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208230932018.png)

### 总结

![image-20250208230955312](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208230955312.png)



## RedisTemplate哨兵模式

![image-20250208231905198](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208231905198.png)

![image-20250208232017215](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208232017215.png)![image-20250208232139350](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208232139350.png)



## Redis分片集群（海量存储，写高并发）

![image-20250208232723660](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208232723660.png)

![image-20250208233043187](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208233043187.png)

![image-20250208233130849](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208233130849.png)

### 散列插槽（重定向）

![image-20250208233346538](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208233346538.png)

![image-20250208233530875](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208233530875.png)

### 集群伸缩（要分配插槽）

![image-20250208233624524](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208233624524.png)

### 故障转移(自动)/数据迁移(手动)

![image-20250208234219602](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208234219602.png)

![image-20250208234413807](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208234413807.png)



## RedisTemplate访问分片集群

![image-20250208234537763](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250208234537763.png)



# 多级缓存

![image-20250209181146157](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209181146157.png)

## JVM(Tomcat+Java)进程缓存

### Caffeine

![image-20250209214355253](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209214355253.png)

![image-20250209214529745](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209214529745.png)

![image-20250209214720895](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209214720895.png)

## Lua(NGINX+Lua)

![image-20250209215651647](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209215651647.png)

![image-20250209215830766](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209215830766.png)

![image-20250209215951939](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209215951939.png)

![image-20250209220151121](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209220151121.png)

![image-20250209220321932](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209220321932.png)



## 多级缓存

### OpenResty

![image-20250209220525652](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209220525652.png)

### NGINX返回请求

#### 快速入门

![image-20250209222345736](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209222345736.png)

![image-20250209222449192](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209222449192.png)

![image-20250209222647601](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209222647601.png)

#### OpenResty获取请求参数

![image-20250209222941619](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209222941619.png)

#### 查询TomCat(先查到TomCat才能进行缓存)

![image-20250209223402728](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209223402728.png)

![image-20250209223555564](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209223555564.png)

![image-20250209223728462](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209223728462.png)

![image-20250209224258375](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209224258375.png)

![image-20250209224415831](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209224415831.png)



#### TomCat集群的负载均衡

![image-20250209224523712](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209224523712.png)

![image-20250209224701287](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209224701287.png)

**hash之后可以在TomCat集群轮询时访问相同端口的TomCat**

### Redis缓存

![image-20250209225001488](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209225001488.png)

![image-20250209225100914](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209225100914.png)

![image-20250209225705604](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209225705604.png)

![image-20250209225803864](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209225803864.png)

### NGINX本地缓存

![image-20250209230316288](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209230316288.png)

![image-20250209230424989](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209230424989.png)

![image-20250209230836088](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209230836088.png)



# 缓存同步

## 同步策略

![image-20250209230927888](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209230927888.png)

![image-20250209231145071](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209231145071.png)

## Canal(康乃偶)

![image-20250209231330870](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209231330870.png)

### 开启MySQL主从

![image-20250209231505312](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209231505312.png)

![image-20250209231736101](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209231736101.png)

### Canal客户端(springboot)

![image-20250209234126741](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209234126741.png)

![image-20250209234300336](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209234300336.png)

![image-20250209234714262](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250209234714262.png)





# Redis实践技巧

## 键值设计

![image-20250210111432583](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210111432583.png)



### BigKey

![image-20250210112108150](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210112108150.png)

![image-20250210111845416](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210111845416.png)

![image-20250210112028511](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210112028511.png)

![image-20250210112354526](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210112354526.png)![image-20250210112417554](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210112417554.png)

![image-20250210112817841](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210112817841.png)

![image-20250210113028054](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210113028054.png)

![image-20250210113220682](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210113220682.png)![image-20250210113328804](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210113328804.png)![image-20250210113520960](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210113520960.png)

![image-20250210113603159](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210113603159.png)



## 批处理

![image-20250210114703354](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210114703354.png)

**MSET只能处理string，  HMSET只能处理hash**

## Pipeline

![image-20250210115001166](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210115001166.png)

![image-20250210115157449](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210115157449.png)

## 集群下的批处理(插槽)

![image-20250210115529227](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210115529227.png)

![image-20250210120013067](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210120013067.png)

**spring封装的**





# 服务端优化

## 持久化配置

![image-20250210120507733](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210120507733.png)

![image-20250210152207982](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210152207982.png)



## 慢查询

![image-20250210152406822](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210152406822.png)

![image-20250210152515142](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210152515142.png)

![image-20250210152702390](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210152702390.png)



## 命令及安全配置

![image-20250210153313800](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210153313800.png)

![image-20250210153322216](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210153322216.png)



## 内存配置

![image-20250210153826194](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210153826194.png)

![image-20250210154004410](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210154004410.png)

![image-20250210154436161](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210154436161.png)



## 集群最佳实践

![image-20250210154716875](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210154716875.png)

![image-20250210154757710](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210154757710.png)

![image-20250210155729253](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210155729253.png)

![image-20250210155828320](C:\Users\wht\AppData\Roaming\Typora\typora-user-images\image-20250210155828320.png)

看               
