# BarChart
----------
BarChart is a javascript class that gives you ability to visualize your data and show it in the bar chart. This class has a lot of options which give it flexibility and also the usage of this class is so simple.

### Features
* Changing the size of chart
* Customize labels
* Define multiple chart
* Each bar has its own color
* Change the background color
* Enable/Disable to show value of each bar
* Adjust the color of value label for each bar
* Dynamically can add a bar to chart
* Show Chart Vertically or Horizontally

### Upcoming Feature
* Change the size of font
* Adding some animations

### Demo
> <a href="https://codepen.io/shahrokhnabavi/pen/KZKPMV" target="_blank">Demo On CodePen</a>


## Getting Started

### Installation & Usage
1. Import the class script into the page.
2. Customize the options <kbd>var options = {}</kbd>
3. Make a new instance of class <kbd>new BarChart( options );</kbd>

### Options
* `container`: the id of canvas tag which is a holder place for the chart.
* `size`: size of chart holder place . the size is an object

	```
	var options = {
		size: { w: 500, h: 250 }
	}
	```
* `label`: this is an object that hold label of each axis
* `data`: An array of objects. Each element of array represents a bar in our chart
* `bgColor`: background color of the chart
* `valueLableEnable`: this is a boolean option, if it be true then for each bar the value of that bar will shown as label inside of that bar
* `valueLableTail`: The value of each bar can be followed by the value of this option
* `isVertical`: If you set this option to true the chart will be shown vertically


**Example**
```
<script type="text/javascript" src="chart.js"></script>
<script type="text/javascript">
    new ChartBar({
        container: "chart",
        size: {w: 500, h: 600},
        label: {x: 'X Axis', y: 'Y Axis'},
        data: [
            {color: 'red', value: 80},
            {color: 'green', value: 20},
            {color: 'blue', value: 100},
            {color: 'silver', value: 50},
            {color: '#fbb', value: 10},
        ]
    });
</script>
```

### License

The BarCart is open-sourced script licensed under the [MIT license](http://opensource.org/licenses/MIT).
