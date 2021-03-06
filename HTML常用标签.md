# HTML常用标签

## ```<a>```标签

### 标签属性
1. href 超链接
2. target 选择打开方式，“_blank”在空白页打开
3. re=noopener
   
href属性中，网址直接写成//xxxxxx.com的形式就可以了，会自动不全协议的。
href后面可以跟网址、地址、伪协议和id。


href=“#xxx”，id可以指向页面上对应的标签。


伪协议分三种，

* JavaScript：代码，其中js代码是指可以直接执行的js代码，然后会在弹出的窗口中显示执行的结果。如果想写一个什么都不做的a标签，那就在href中写入一个空的js伪协议
```html
<a href:"javascript:;"></a>   这个a标签可以不刷新页面，也不让页面翻滚，维持原状
``` 

* mailto：邮箱，可以指向发邮件的链接，唤起默认的邮箱系统
* tel：电话，可以直接打电话，这个在手机端很好使用，直接唤起拨号界面，把号码填写在界面上
  
-----------

### target值

 * _blank
 * _self
 * _top 最顶层页面打开，涉及到iframe页面之间相互引用。
 * _parent 在父级窗口打开，这也涉及到页面之间的相互引用
 * xxx 如果没有xxx则创建一个xxx窗口，如果有就在xxx窗口打开新的页面

------------

## ```<img>```标签

```<img>```标签，发出get请求，展示一张图片

### 标签属性：
* alt ，当图片请求失败时显示
* width
* height ，宽和高，如果只写其中一个属性，另一个属性会根据情况按比例自适应
* src 图片源地址

-----------
注意事项：在手机上响应页面的时候，需要在reset里面写```img{ max-width：100% }```，就可以让图片的宽占满手机屏幕，是一个响应式的标签。


## ```<table>```标签

```<table>``` 标签下一级只会有三个标签分别是：

* ```<thead></thead>``` 
  
  下一级标签有```<tr></tr>``` 、```<th></th>```、```<td></td>```  
  无论是双表头还是单表头，表头用th表示，数据用td表示
  

* ```<tbody></tbody>```
* ```<tfoot></tfoot>```


------------
table 标签其他样式，（CSS知识）
* table-layout 
* border
* border-spacing
* border-collapse