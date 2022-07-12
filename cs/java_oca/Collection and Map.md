# Collection and Map
https://tech.meituan.com/2016/06/24/java-hashmap.html
## Big Picture
![Collection and Map](https://www.ictdemy.com/images/1/java/collections/java_collection_api_diagram.svg)
![Collection and Map](https://www.runoob.com/wp-content/uploads/2014/01/2243690-9cd9c896e0d512ed.gif)

    public interface Map<K,V> {
            ...
            Set<K> keySet();
            Collection<V> values();
            ...
    }

Map 主要有四个实现类

HashMap, Hashtable, LinkedHashMap, TreeMap

## HashMap

根据key的hashCode值存储数据，大多数情况下可以直接定位到它的值，因而具有很快的访问速度，但遍历顺序却是不确定的。HashMap最多只允许一条记录的key为null，允许多条记录的值为null。HashMap非线程安全，即任意时刻可以有多个线程同时写HashMap，可能会导致数据的不一致。如果需要满足线程安全，可以使用Collections的synchronizedMap 方法使HashMap转为线程安全，或者使用ConcurrentHashMap。

## Hashtable

Hashtable是遗留类，继承自Dictionary类，并且线程安全。不建议使用。

## LinkedHashMap

LinkedHashMap是HashMap的一个子类，保存了记录的插入顺序，在用Iterator遍历LinkedHashMap时，先得到的记录肯定是先插入的，也可以在构造时带参数，按照访问次序排序。

## TreeMap

TreeMap实现SortedMap接口，能够把它保存的记录根据key排序，默认按key升序排序，也可以指定排序的比较器，当用Iterator遍历TreeMap时，得到的记录是排过序的。如果使用排序的映射，建议使用TreeMap。在使用TreeMap时，key必须实现Comparable接口或者在


## HashMap 内部实现

搞清楚HashMap，首先需要知道HashMap是什么，即它的存储结构-字段；其次弄明白它能干什么，即它的功能实现-方法。

从结构实现来讲，HashMap是数组+链表+红黑树（JDK1.8增加了红黑树部分）实现的，如下如所示。

![HashMap](https://awps-assets.meituan.net/mit-x/blog-images-bundle-2016/e4a19398.png)