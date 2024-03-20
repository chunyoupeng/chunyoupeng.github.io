# 背景

美国国防部(DoD)在过去有大量的不同数据标准、协议的系统。STITCHES就是为了实现系统在不需要共享公共标准的情况下实现实现互操作的一个系统.而子系统可以根据自已的需求独立开发而不受影响.

# 节点的传输

Transforms Expressed in a Domain Specific Language Built for this Purpose

点节的数据的传输是由定义在它上面的DSL进行的.


# 结构图

![](/home/dell/Pictures/Screenshots/Screenshot%20from%202024-03-05%2016-22-20.png)

中间有一部是把配置文件转换成C++/Java代码,这一步就有我们做的非常相似.


# DSL

![](/home/dell/Pictures/Screenshots/Screenshot%20from%202024-03-05%2017-02-52.png)

- 提供高层的函数, 嵌套的表达式, 语法糖
- 提供了类型系统
- 辑写人可以直接读的语言

# Config file 

![](/home/dell/Pictures/Screenshots/Screenshot%20from%202024-03-05%2017-10-04.png)

把上面的配置文件转换成对应的代码.
