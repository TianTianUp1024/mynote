1. 数据库的使用语句 MySQL：表整合
2. 基本的排序算法：快速排序
3. 数据结构：已知前序遍历求后序遍历
4. 实习生：数据库 表  项目一数据表怎么设计
5. 服务 美食 娱乐  不应该用外键 有很多问题
6. MySQL 学习！ 
7. 自己建表一下，实习生知道了数据库表的话就知道了业务的大部分流程。项目一的数据库表示非常关键。只要表现的比其他人好就行，满分100分，拿了10分 其他人都是5分 选的就是你，放心。
首先，先建表一行：服务 美食 娱乐 
再将一个表 住宿表 ID列 name列 proID列 链接上表的服务ID（例如上表的是1 那这里也指定1）
proID，不用外键，建一个新的列去连接表
外键有很多不好的地方，用改键方法更好
8. solr  memcached
9. 技术在项目中的具体应用场景 ，只要知道某个项目的具体应用场景并说是自己在项目中就这么用的就行
10. 文档中没有的有的面经上有：例如MySQL如何优化
11. 实习
12. 项目里5 6个人 中途有人离职
一个项目交付给客户之后马上另一个项目就来了，上线，没什么BUG，在开发的过程中，每天都会开会，组长分配当天的任务，以及遇到什么问题和难点在开会的时候解决，每天都会发总结报告
有很多问题都是解决讨论出来的，具体项目库建表 有些难的设计东西 有些犹豫不决的去问组长 整个项目的整体架构由架构师来完成的
13. 关于不用外键
1：在大数量的情况下，使用外键约束会导致很差的性能。一般互联网应想都不要去想外键这种东西了，连表连接查询最好都不要使用
2：大数据量时进行表的水平切分，像外键约束、触发器、存储过程这些都是禁区
3：数据完整性是业务的需要，因此得由业务层的应用程序来控制
4：外键会导致表结构非常混乱，几乎是动都不能去动，一层套一层的外键约束，在表很多的情况下很可能会导致循环约束

1. 为什么使用solr而不使用ElasticSearch作为全文搜索引擎？
服务场景不同，这是传统搜索与实时搜索的区别

传统搜索是从静态数据库中筛选出符合条件的结果，这种结果往往是不可变得、静态的。而实时搜索则是说用户对于搜索的结果是实时变化的。

传统搜索比如电商这种，实时搜索参考谷歌，百度，这种实时搜索。

2. 