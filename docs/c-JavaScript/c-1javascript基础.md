## 1. JS中的变量和类型
### 1.1 基本数据类型

JS中有6中基本数据类型，分别是：
- boolean
- number
> number中有一个特殊的NaN，代表不都是一个有效数字，但是是属于number。
- string
- null
- undefined
- symbol

### 1.2 null是OBject吗？
虽然`typeof null`会输出object，但是这只是JS中存在的一个悠久的bug，在JS的最初版本中使用的是32位系统，为了性能考虑使用低位存储变量的类型信息，000开头代表对象，然而null表示全为零，所以将它错误的判断为object，虽然现在的内部类型判断已经改变了，但是对于这个Bug却是一直流传下来。

### 1.3 原始值和引用值的区别
> 原始值: null, undefined, string, number, boolean, symbol   
引用值：Object,Array,Function,RegExp,Date

- 存储位置的不同    
(1)原始类型存储的是值，对象类型存储的是地址。
原始类型的空间是固定，存储在较小的内存域——栈中，便于快速查找变量值。   
(2)引用类型存储在堆中，这个对象在堆中的地址存储在栈中。

- 赋值的方式不同    
(1)原始值赋值：拷贝值的副本给新的变量，两个变量相互独立，改变其中一个值不会影响另一个值   
(2)引用值赋值：将引用传递给新的变量，实际上就是将地址引用赋值给新的变量，两个变量指向同一个地址，也就是指向堆中的同一个区域，改变其中一个值，另一个值也会随着改变。

> 持续更新中...







> 参考：https://blog.nowcoder.net/n/0a853b4e56a544f8933d171f0adf8756    
>https://github.com/huyaocode/webKnowledge/blob/maste

