## 8.1 单元测试 -Jasmine-
&emsp;&emsp;测试是提升应用品质不可或缺的工作。在JavaScript的世界中也不例外。特别是近年来伴随着客户端功能的比重越来越高、在JavaScript中也普遍使用面向对象编程、写的脚本也更加复杂了。为了确保脚本的品质，需要在JavaScript中实施测试——然后，就必须要引入用来支援测试的测试框架。<br>
&emsp;&emsp;测试的大致分类如下。
- 单元测试 → 检查函数／类（方法）的动作  
- 结合测试 → 检查多个函数／类（方法）结合时的动作
- 系统测试 → 检查应用整体的动作

&emsp;&emsp;测试框架主要是支援其中的单元测试（Unit Testing）的部分的。有如下比较有名的JavaScript中可以使用的测试框架，本书采用当前时间点市场份额最高的，相关文档最齐全的Jasmine。
![image](../../images/c8/スクリーンショット&#32;2019-04-19&#32;午前11.22.21.png)
&emsp;&emsp;使用测试框架，我们可以更简单地，并且以统一的规则来创建测试代码。