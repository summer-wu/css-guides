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

## css selector语法体验
+ [./selector-familiar.html](./selector-familiar.html)

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