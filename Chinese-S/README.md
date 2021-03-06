# GitHub 傻瓜手把手教程

目录
[用GitHub提交修改申请到原文](#commit)

GitHub界面超难用有木有！每个名字都取的很高深看不懂有木有！查出来的解释也很高深还是看不懂有木有！

没事！

这篇教程就是来帮你轻轻松松学会GitHub的！  
0基础也没问题！

那我们现在就开始吧！

## GitHub有啥用捏？

GitHub让你可以与别人**轻轻松松地**合作完成一份文件。

通常这个文件指的是代码，但你也可以用它来写书、写文章。（注：其实有个网站叫[GitBook](https://www.gitbook.com) 是专门让一群人合作写书的。。和GitHub原理一样。）

假如你用过Google协作文档的话，你就知道一群人一起完成一份文件真的是一件很酷的事情！

但是很多人同时编辑一份文件会很混乱，想象一下假如一个文件里有一行字：
```
豆腐脑
```

两个人看到了，都觉得要加个形容词才行  
但一个人改成了
```
咸的豆腐脑
```

而另一个人则改成了
```
甜的豆腐脑
```

这时候两个改变就打架了！

而GitHub背后的机制Git就是专门为了解决这个问题而生的！

作为文件主人的**Master大老板**会看到Git系统跟他说

**$System** \> _打架咯！_  
_**North北北**做出了改变如下_  
```diff
- 豆腐脑
+ 咸的豆腐脑
```
_并说到：“豆腐脑咸的才有家乡味！”_  
_**South南南**做出了改变如下_  
```diff
- 豆腐脑
+ 甜的豆腐脑
```
_并说到：“豆腐脑加糖水才是王道！！”_  
_请在下面写出你想做的改变：_  
**$Master大老板** \>
```
普通的豆腐脑
```
**$System** \> _为此改变写个注释呗：_  
**$Master大老板** \> 你俩别争了！再吵明天一起去人事部领工资！  

解决啦。

不过呢，要是**Master大老板**每天都要处理每一个小打架的话，那还不得把全公司人给开除了

实际上，GitHub很少会真正的发生打架。因为大部分时候，每个人对文件的修改请求都是有先后顺序的。

在一个人发出修改请求时，GitHub会找出被做出的修改并且把修改标记出来

比如说，假如**North北北**先提交了修改，
系统会问他：

**$System** \> _您即将提交修改如下：_  
```diff
- 豆腐脑
+ 咸的豆腐脑
```
_为此请求写个注释呗？_  
**$North北北** \>  豆腐脑咸的才有家乡味！  
**$System** \>  _确定提交修改吗？是/否_  
**$North北北** \> 是  

（斜体为系统输出，正常字体为**North北北**的输入)

而之后**South南南**再提出修改时就会看到

**$System** \> _您即将提交修改如下：_  
```diff
- 咸的豆腐脑
+ 甜的豆腐脑
```
**$System** \> _为此请求写个注释呗？_  
**$South南南** \> 胡说！豆腐脑怎么会是咸的！太逆天了！  
**$System** \> _确定提交修改吗？是/否_   
**$South南南** \> 是  

虽然这样**Master大老板**不会被系统提醒烦到，  
但他俩这样乱改原文件还是会被开除对吧\_(:3」∠)\_。。。  

所以GitHub其实提供了其他方法可以让你把原文件复制一份，做出修改，再一次向大老板请求合并到原文件的。  
这个方法叫做Branch(分支)。

但看新方法之前我们先看看如何用GitHub实现我们的方法一：**提交修改申请到原文件**。

## 用GitHub提交修改申请到原文（也就是所谓的Commit<a name="commit"></a>）

首先看一下浏览器的网址列，确定你现在在[https://github.com/ghcpuman902/GitHub-Step-By-Step-Tutorial/tree/master/Chinese-S](https://github.com/ghcpuman902/GitHub-Step-By-Step-Tutorial/tree/master/Chinese-S),滚到页面最上面。

假如不在的话，点击[这里](https://github.com/ghcpuman902/GitHub-Step-By-Step-Tutorial/tree/master/Chinese-S)打开。

确定你有GitHub账号且登陆了。

1. 点击来打开`南北撕逼.txt`，如图所示
![commit step 1 - oepn text file](img/commit_step_1_oepn_text_file.jpg)
可以在图片中看到左上角有一本書的圖標右邊寫著：ghcpuman902/GitHub-Step-By-Step-Tutorial，ghcpuman902是我，這個項目目錄創建者的用戶名。  
後面跟著的GitHub-Step-By-Step-Tutorial就是這個項目的名字啦。

2. 点击小铅笔（Edit this file）图标，对文件进行编辑。
![commit step 2 - edit text file](img/commit_step_2_edit_text_file.jpg)

3. 在每个食物下面写下你喜欢的吃法
![commit step 3 - editing text file](img/commit_step_3_editing_text_file.jpg)


