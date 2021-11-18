# CSS入门分享

## css基础语法规则
+ ![](./imgs/03-selectors.png)
```
style-rule ::=
    selectors-list {
      properties-list
    }
```
+ 常用的selector有`* p .classname #idname`
+ 比如这段 `p{font-size:20px;}`
+ [property和attribute的区别](./property-vs-attribute.md)

### css selector语法体验
+ 空格和逗号的区别：空格表示descendant，逗号是separator并列。
+ 记不住？只需要记住csv，comma separated value。这里是comma separated selectors
+ [./selector-familiar.html](./selector-familiar.html)
+ 体验1 使用多种方式
<pre color="white">

.box0 .div0{color:red}
.box0 .div1{color:blue}
.box0 div{color:green;}

.box0>.div0{color:red}
.box0>.div1{color:blue}
.box0>div{color:green;}

.box0 div:nth-child(2){color:red}
.box0 div:nth-child(3){color:blue}
.box0 div{color:green}

</pre>
+ 体验2 多种方式
<pre style="color:white">
.p0,.p2,.p4{background:gray}
.p1,.p3,.p5{background:white}

.box1 p:nth-child(2n){background:gray}
.box1 p:nth-child(2n+1){background:white}

.box1 p{background:white}
.box1 p:nth-child(even){background:gray}
</pre>
> nth-child实际是count start 1，可以尝试把pre注释掉试一下。


## css cascading体验
+ [cascading.md](./cascading.md)
## css布局

## flex布局

## 技巧 居中

## css发展趋势
+ css variables，chrome已经支持
+ less/sass，预处理，支持嵌套和变量
+ module css，在webpack中引用
+ styled-component，react生态中最流行的css-in-js解决方案
