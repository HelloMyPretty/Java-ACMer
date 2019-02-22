1. # Java与算法相关常用知识

    从网上摘录，总结了一些java与算法常用的类库api，对一些使用java做acm、刷算法题的初学者十分有用。内容包括常用的容器类以及与之相关工具类、实现`Comparable`接口，重写`equals`方法、字符串等做了简要介绍。
    对于其中的某些知识点给出了相应的原理介绍，这是为了更好的理解使用，如果有Java基础的看一下应该能明白。
    对于各个容器的各个接口给出了常用实现类的简要介绍，由于Java继承机制——实现类方法与其基类接口大多相同，当我们了解接口方法之后就能熟练应用实现类方法，因此我在每个接口的实现类后面给出了接口方法的**常用api**。
    在介绍Queue与Deque接口时，由于Java提供了两套功能相同，返回类型不同的方法。为了方便记忆这里只介绍了常用的一套，它们的方法名更能体现其功能。

    由于时间仓促，技术原因，若有错误还望指出；所有内容均来自互联网，并在**参考资料**列出参考博客。

    主要内容如下：

    ## Java容器类接口框架总览

    1. Collection接口 

       1.1. Collection主要方法 

       1.2. Collection对集合运算的支持 

       1.3. Collection转化为数组toArray() 

    2. List接口 

       2.1. List主要方法 

    3. Queue与Deque接口

       3.1. Queue 主要方法 

       3.2. Deque 主要方法

       3.3. 主要实现类

    4. Map接口 

       4.1. Map的主要方法 

       4.2. Map.Entry键值对 

       4.3. SortedMap接口 

       4.4. NavigableMap接口

    5. Set接口

       5.1. SortedSet接口 

       5.2. NavigableSet接口

    6. 实现类小结

    7. 迭代器

       7.1. Iterable

        7.2. Iterator  

          7.2.1. Iterator主要方法

          7.2.2. 游标模式

          7.2.3. fail-fast机制 

       7.3. ListIterator 

          7.3.1. ListIterator主要方法 

    ## 常用工具类库

    1. Collections类 
    
    2. Arrays类 
    
    3. Math类 
    
    4. BigInteger类 
    
    5. Random类 
    
    6. Scanner类 
    
    7. System.out

    ## 字符串

    1. String类 

       1.1. 构造方法

       1.2. String的不可变形 

       1.3. String.format 

       1.4. String的常用方法 

       1.5. String与正则表达式

          1.5.1 正则表达式简介

          1.5.2. 常用的正则表达式词法  

          1.5.3. 正则示例       

          1.5.4 String.matches()匹配正则表达式 

          1.5.5 String.split() 从正则表达式匹配的地方分离

          1.5.6 替换与正则表达式匹配的地方

    2. StringBuilder类 

       2.1. StringBuilder的构造方法

       2.2. StringBuilder的常用方法

    3. 基本数据类型与字符串的转换

       3.1. 基本类型转换为字符串

       3.2. 字符串转化为基本类型

    ## 实现元素比较

    1. ==、equals、compareTo的关系

    2. 重写equals方法 

       2.1. equals重写的规范

       2.2. 为什么重写equals的同时还得重写hashCode

       2.3. 快速生成hashCode和equals

          2.3.1 使用Objects的静态方法

          2.3.2 IDEA自动生成hashCode与equals的方式

       2.4. 总结

    3. Comparable接口自然排序

       3.1. 规范

       3.2. 示例

    4. comparator定制排序 

       4.1. 示例

    5. 重写equals方法的标准套路 

    6. 重写hashCode的标准套路

    7. 参考资料

    ## Collection下主要接口实现类

    1. List实现类

       1.1. ArrayList

       1.2. LinkedList

    2. Map实现类

       2.1. HashMap

       2.2. TreeMap

    3. Queue实现类

       3.1. ArrayDeque

       3.2. PriorityQueue 

    4. Set实现类

       4.1. HashSet

       4.2. TreeSet
