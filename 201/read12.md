# Chart in JS
**What Chart mean?**
*chart is a graphical representation for data visualization, in which "the data is represented by symbols, such as bars in a bar chart, lines in a line chart, or slices in a pie chart". A chart can represent tabular numeric data, functions or some kinds of quality structure and provides different info.*

**The chart in JS**
*We have step to create the chart:*
-Setting up : by download Chart.js then copy it into HTML code
-Drawing a line chart:the first create  element in HTML
-Drawing a pie chart
-Drawing a bar chart
--------------------------------------------------
# Canvas
-**Canvas it's element tage in HTML we can use it to crate a chart then modifiy that chart**
**The HTML <canvas> element is used to draw graphics on a web page**
-**It shows four elements: a red rectangle, a gradient rectangle, a multicolor rectangle, and a multicolor text**
-**crate the HTML canvas tage and give it the attrbuite like id,hight,width****
-**we must add JS and we can draw line,circle and we can draw a Text,Stroke Text,Draw Linear Gradient,Draw Circular Gradient** 
###### Example in some Canvas chart from (canvasjs.com)
<!DOCTYPE HTML>
<html>
<head>
<script type="text/javascript">
window.onload = function () {

var chart = new CanvasJS.Chart("chartContainer", {
	theme: "light1", // "light2", "dark1", "dark2"
	animationEnabled: false, // change to true		
	title:{
		text: "Basic Column Chart"
	},
	data: [
	{
		// Change type to "bar", "area", "spline", "pie",etc.
		type: "column",
		dataPoints: [
			{ label: "apple",  y: 10  },
			{ label: "orange", y: 15  },
			{ label: "banana", y: 25  },
			{ label: "mango",  y: 30  },
			{ label: "grape",  y: 28  }
		]
	}
	]
});
chart.render();

}
</script>
</head>
<body>
<div id="chartContainer" style="height: 370px; width: 100%;"></div>
<script src="https://canvasjs.com/assets/script/canvasjs.min.js"> </script>
</body>
</html>



![canvas](https://i.stack.imgur.com/642Ei.png)
