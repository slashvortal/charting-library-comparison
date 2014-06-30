# Charting Library Comparison

A variety of test pages for performance analysis of various charting libraries with ops/second logged to the console.

## Streaming Line Charts
Minimal configuration, no axis or grid lines, attempting to redraw as fast as possible (setTimeout(draw, 0)) with one data pushed and one data shifted out with each draw (1,000 points to draw are maintained at all times).

* [D3](http://ozan.io/charting-library-comparison/d3/streaming-line-chart.html) - Popular, well-designed, svg-based.
* [Highcharts](http://ozan.io/charting-library-comparison/highcharts/streaming-line-chart.html) - Popular, feature-rich, svg-based, slow.
* [Dygraphs](http://ozan.io/charting-library-comparison/dygraphs/streaming-line-chart.html) - Canvas-based, over 5 years old, code is a bit soupy but seems well tested.
* [Rickshaw](http://ozan.io/charting-library-comparison/rickshaw/streaming-line-chart.html) - A sugar layer on top of D3 to enable reusable charts.
* [Chart.js](http://ozan.io/charting-library-comparison/chartjs/streaming-line-chart.html) - I think I'm missing something with this framework (because it's so popular for being so young), but it seems very poorly designed.
* [Plain Canvas](http://ozan.io/charting-library-comparison/custom/streaming-line-chart.html) - Baseline benchmark drawing lines directly to canvas
