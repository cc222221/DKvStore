# kvStorage
# 一、项目主要功能和知识点
参照redis，主要实现的功能：  
1、数据的插入、查询、删除等操作  
1）SET：插入key - value  
2）GET：获取key对应的value  
3）COUNT：统计已插入多少个key  
4）DELETE：删除key以及对应的value  
5）EXIST：判断key是否存在  

2、实现不同的数据结构存储引擎  
不同的数据结构，操作的效率是不一样的。因此我们实现基于数组array、红黑树rbtree、哈希hash、跳表skiptable 这四种数据结构，实现kv存储，并测试相应的性能。  

3、测试用例  
1）功能测试  
2）10w的qps测试  
 
4、主要涉及的知识点有  
1）基于协程，一个连接对应一个协程  
2）tcp网络交互  
3）数据结构：数组array、红黑树rbtree、哈希hash、跳表skiptable、动态哈希dhash 

5、优化的空间是
1）加入日志
2）数据持久化和重放功能
3）分布式，支持集群

