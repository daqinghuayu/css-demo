#transition
语法
```
transition: property duration timing-function delay;
```
实例
```
    -webkit-transition: color .2s ease-out 1s;
    -moz-transition: color .2s ease-out 1s;
    -o-transition: color .2s ease-out 1s;
    transition: color .2s ease-out 1s;
```

transition 属性是一个简写属性，用于设置四个过渡属性：
```
1.transition-property           规定设置过渡效果的 CSS 属性的名称。
2.transition-duration           规定完成过渡效果需要多少秒或毫秒。
3.transition-timing-function    规定速度效果的速度曲线。
4.transition-delay              定义过渡效果何时开始。
```


1.transition-property: none|all|property;
```
none        没有属性会获得过渡效果。
all         所有属性都将获得过渡效果。
property    定义应用过渡效果的 CSS 属性名称列表，列表以逗号分隔。
```

2.transition-duration: time;
```
time        规定完成过渡效果需要花费的时间（以秒或毫秒计）。
            默认值是 0，意味着不会有效果。
```

3.transition-timing-function: linear|ease|ease-in|ease-out|ease-in-out|cubic-
bezier(n,n,n,n);
```
linear      规定以相同速度开始至结束的过渡效果（等于 cubic-bezier(0,0,1,1)）。
ease        规定慢速开始，然后变快，然后慢速结束的过渡效果（cubic-bezier(0.25,0.1,0.25,1)）。
ease-in     规定以慢速开始的过渡效果（等于 cubic-bezier(0.42,0,1,1)）。
ease-out	规定以慢速结束的过渡效果（等于 cubic-bezier(0,0,0.58,1)）。
ease-in-out	规定以慢速开始和结束的过渡效果（等于 cubic-bezier(0.42,0,0.58,1)）。
cubic-bezier(n,n,n,n)   在 cubic-bezier 函数中定义自己的值。可能的值是 0 至 1 之间的数值。
```
三次贝塞尔
http://cubic-bezier.com/

4.transition-delay: time;
```
time    规定在过渡效果开始之前需要等待的时间，以秒或毫秒计。
```