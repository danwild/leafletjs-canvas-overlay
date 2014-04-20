Leaflet Canvas Overlay - straightforward full screen canvas overlay that calls custom user function for drawing

		//Example:
		L.canvasOverlay()
		   .params({data: points})     // add any custom data that will be passed to draw funciton
	           .drawing(drawingOnCanvas)   // set drawing funciton
	           .addTo(leafletMap);         // add this layer to leaflet map
	            

		//Custom drawing function:
			function drawingOnCanvas(canvasOverlay, params) {
		            var ctx = params.canvas.getContext('2d');
		            params.options.data.map(function (d, i) {
		              // canvas drawing goes here
		            });
		        };

Other useful Leaflet Canvas sources here:
(Full Canvas) [https://github.com/cyrilcherian/Leaflet-Fullcanvas]


