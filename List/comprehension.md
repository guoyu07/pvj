###列表解析 列表生成式

不知道用哪个名字 我看的书和网上的教程用的名称是不一样的 英文是：List Comprehensions
一个绝对变态强大的东西 用它可以非常快速的创建列表
上代码~

```python
#1 -10 的平方
[n * n for n in range(1, 11)]

#后面加上判断 生成仅为偶数的平方
[n * n for n in range(1, 11) if n % 2 == 0]
#输出 [4, 16, 36, 64, 100]


#双循环 就是这么智能 生成全排列
[m+n for m in 'as' for n in '12']
#['a1', 'a2', 's1', 's2']

#双参数循环一个dict  给劲
d = {'x': 'A', 'y': 'B', 'z': 'C' }
[k + v for k,v in d.items()]
#['yB', 'xA', 'zC']
```

关于js的写法 好消息是 我们伟大的es6居然支持 数组生成式了~ es6好多新东西都是和python一模一样的 不过es6能真正推广使用至少要5年

```javascript
var a = [1, 2, 3, 4];
var b = [for(i of a) i*2];
//输出 [2, 4, 6, 8]

//再加点if条件
var a = [3, 10, 11, 15];
var b = [for(i of a) if (i>10) i*2];
//输出 [22, 30]
```


