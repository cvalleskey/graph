Graph
=========================

A lightweight, library agnostic plugin for displaying dynamic (or static) data using the <canvas> element.

How does it work?
-----------------

Graph makes use of the HTML5 <canvas> tag, a nifty little thing that lets you draw content onto it via JavaScript. View the <a href="http://chrisvalleskey.com/graph/">demo</a> to see some of the options it has.


Prerequisites
-------------

* Nothing!


Usage
-----

* Download the graph.js file
* Invoke graph() on your <canvas> element, like so:

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


Customization
-------------
