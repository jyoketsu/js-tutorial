##### 【379页】
# 7.3 保存用户数据 -Storage对象-
&emsp;&emsp;在JavaScript的世界中，原则上是不允许使用脚本随意向计算机中写入的。这是因为如果用户在访问网站时替换了计算机中的文件就严重了。<br>
&emsp;&emsp;作为这个例外的方法，在初期浏览器提供了一个叫做「cookie」的结构。在Web应用中，使用cookie可以保存客户端的小体积文本。<br>
&emsp;&emsp;不过，使用JavaScript很难操作这个cookie并且还有大小的限制。因此现在推荐使用Web Storage（本地存储）来代替。<br>
&emsp;&emsp;本地存储是指浏览器内置的数据存储（库）。使用特定的键值组合来保存数据，所以也称为Key - Value型数据存储。

Key（键）|Value（值）
:--|:--
fruit1|苹果
fruit2|柑橘
fruit3|葡萄
……|……

根据键来决定值的唯一性  
可以管理简单的数据  
**●什么是Web Storage**

&emsp;&emsp;下面，我们来看下cookie和本地存储的差异。

项目|本地存储|cookie
:--|:--|:--
数据大小的上限|大（5MB）|小（4KB）
数据的有效期|无|有
数据通信|无|请求时，也发送给服务器

**●本地存储和cookie的差异**

&emsp;&emsp;下面是本地存储的基本用法，我们一边看示例一边介绍。