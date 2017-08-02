<p align="center">
  <a href="https://github.com/pkwenda/gantt.js/blob/master/LICENSE"><img src="https://img.shields.io/badge/license-MIT-4EB1BA.svg?style=flat-square" alt="Build Status"></a>
   
  
  <a href="#"><img src="https://img.shields.io/badge/version-0.0.1-red.svg?style=flat-square" alt="Sauce Test Status"></a>
</p>

## gantt.js
甘特图 插件 依赖 jQuery.js date.js

- 两条线的甘特图[预期值]+[实际值] 插件
打破传统甘特图一条线的模式，采用`计划`和`实际`两条线，更加直观，并去掉一些拖动组件。
- 不靠svg这种比较笨重的组件，完全hml元素生成
- 源码小，轻量级

- todo：汉化+响应式

- Example

```
$("#ganttChart").ganttView({ 
  data: ganttData, //数据源
  slideWidth: 600, //定义大小，默认400
  behavior: {
    onClick: function (data) { //绑定点击事件
    console.log(data);
  }
});			 	 
```
 
![Alt text](example/image.png "gantt")


