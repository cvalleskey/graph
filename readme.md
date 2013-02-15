Graph
=========================

A lightweight, library agnostic plugin for displaying dynamic (or static) data using the `<canvas>` element.

How does it work?
-----------------

Graph makes use of the HTML5 <canvas> tag, a nifty little thing that lets you draw content onto it via JavaScript. View the <a href="http://chrisvalleskey.com/graph/">demo</a> to see some of the options it has.


Usage
-----

	<script type="text/javascript" src="js/cv_graph.js"></script>
	<script type="text/javascript">
	window.onload = function() {
		g_graph = new Graph(
		{
			'id': "firstgraph",
			'strokeStyle': "#819C58",
			'fillStyle': "rgba(64,128,0,0.25)",
			'call': function(){return ( Math.floor(Math.random()*50 + 25));}
		});
	}
	</script>
	<canvas id="firstgraph" width="620" height="150"></canvas>
	

Customization
-------------

	var default_args = {
		'id': "graph", // ID of the <canvas> element
		'interval':	300, // Refresh rate in milliseconds
		'showline':	true, // Draw line
		'showfill':	true, // Draw fill
		'lineWidth': 2, // Width of the line
		'strokeStyle': "#666", // Color of the line
		'gridcolor': "#EEE", // Color of the grid
		'background': "#F9F9F9", // Color of the background
		'fillStyle': "rgba(0,0,0,0.25)", // Color of the fill
		'showdots':	true, // Show data points as dots
		'showgrid': true, // Show the grid
		'showlabels': true, // Show labels for each data point
		'grid': [10,10], // Grid dimensions
		'range': [0,100], // Range of the graph
		'call': function(){return Math.floor(Math.random()*100) + 50;} // Function from which data is obtained
	}
