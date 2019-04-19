# 7.6 在后台运行JavaScript的代码 -Web Worker-
&emsp;&emsp;JavaScript基本上是单线程的。也就是说在JavaScript中一次只能进行一个工作。因此，一旦JavaScript中发生了所谓的繁重的操作，页面的动作就会经常发生卡顿。<br>
&emsp;&emsp;但是，使用Web Worker这个功能，便可以使JavaScript的代码在后台并行地运行。这样，即使是在处理繁重处理的过程中，用户也可以在浏览器中继续操作。
![image](../../images/c7/スクリーンショット&#32;2019-04-19&#32;午前8.42.56.png)
> 繁重的处理  
> 其他处理  
> postMessage方法  
> 将处理交给其他线程  
> 将结果回传给主线程  
> worker  
> 在后台执行JavaScript处理

**●什么是Web Worker**

&emsp;&emsp;另外，可能有读者会认为「使用setTimeout方法，不也可以同样地并行执行处理吗？」，但这其实是一个误解。使用setTimeout方法设定的工作，只要一旦把它放在一边，结果还是只是在一个线程上依次处理（这就是之前为什么说「使用setTimeout方法设定的时间是不正确的」）。setTimeout方法最多只能是模拟并行处理。

**Note 什么是线程**<br>
&emsp;&emsp;线程（thread）是执行程序的处理的最小单位。在英语中是「线」的意思，通常的程序就是由多个这样的线程（线）合成的一根结实的带子（功能），这样想象会更容易理解。<br>
&emsp;&emsp;「JavaScript是单线程的」是指这个线程通常只有1个（=使用1根线运行）。相对于单线程，多个线程运行的处理称为多线程处理。Web Worker是将JavaScript处理多线程化的功能。