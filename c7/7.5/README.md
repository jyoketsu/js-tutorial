##### 【411页】
# 7.5 简单显示异步处理 -Promise对象-
&emsp;&emsp;在JavaScript中执行异步处理，有经典方法之一的回调函数（4.6.3）。目前为止，我们在setTimeout／setInteval方法、XMLHttpRequest对象等各方面使用了回调函数。也可以说是JavaScript方言。<br>
&emsp;&emsp;但是，如果有连续多个异步处理时，回调函数的嵌套就会很深，1个函数就会变得很臃肿。我们将这样的问题称为回调地狱。
![image](../../images/c7/スクリーンショット&#32;2019-04-17&#32;午後9.39.37.png)

&emsp;&emsp;
●／・■→×÷※
①②③④⑤

7.5.1 掌握Promise对象的基础
7.5.2 连接异步处理
7.5.3 使多个异步处理并行
7.6 在后台运行JavaScript的代码 -Web Worker-
7.6.1 实现worker线程
7.6.2 启动worker线程

原文|译文|备注
:--|:--|:--