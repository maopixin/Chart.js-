## 确保Chart.js文件引入成功 并且DOM中有一个canvas元素


```javascript
// 1.获取canvas元素的实例化对象
const context = document.getElementById('myChart').getContext('2d');
// 2.获取chart的实例化对象（他是面向对象的，可以实例化 ， 并且在全局中暴露了一个    ***Chart***   的变量）
const myNewChart = new Chart(ctx);
//配置数据

const data = {
	labels : ["1月","2月","3月","4月","5月","6月","7月"],
	datasets : [
		{
			fillColor : "rgba(220,220,220,0.5)",
			strokeColor : "rgba(220,220,220,1)",
			pointColor : "rgba(220,220,220,1)",
			pointStrokeColor : "#fff",
			data : [65,59,90,81,56,55,40]
		},
		{
			fillColor : "rgba(151,187,205,0.5)",
			strokeColor : "rgba(151,187,205,1)",
			pointColor : "rgba(151,187,205,1)",
			pointStrokeColor : "#fff",
			data : [28,48,40,19,96,27,100]
		}
	]
};
//通过实例化对象下的Line方法 ，并且传入上面声明的data对象
myNewChart.Line(data);

//现在你应该可以看到效果了

```