# gantt.js
甘特图 插件 依赖 jQuery.js date.js

- 两条线的甘特图[预期值]+[实际值] 插件
打破传统甘特图一条线的模式，采用`计划`和`实际`两条线，更加直观，并去掉一些拖动组件。

- Example

```
$(function () {
			$("#ganttChart").ganttView({ 
				data: ganttData, //数据源
				slideWidth: 600,
				behavior: {
					onClick: function (data) { 
						var msg = "You clicked on an event: { start: " + data.start.toString("M/d/yyyy") + ", end: " + data.end.toString("M/d/yyyy") + " }";
						$("#eventMessage").text(msg);
					},
					onResize: function (data) { 
						var msg = "You resized an event: { start: " + data.start.toString("M/d/yyyy") + ", end: " + data.end.toString("M/d/yyyy") + " }";
						$("#eventMessage").text(msg);
					},
					onDrag: function (data) { 
						var msg = "You dragged an event: { start: " + data.start.toString("M/d/yyyy") + ", end: " + data.end.toString("M/d/yyyy") + " }";
						$("#eventMessage").text(msg);
					}
				}
			});
			
			// $("#ganttChart").ganttView("setSlideWidth", 600);
		});
```
 
![Alt text](example/image.png "gantt")


