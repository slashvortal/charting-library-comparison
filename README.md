# Charting Library Comparison

A variety of test pages for performance analysis of various charting libraries with ops/second logged to the console.
The a brief intro to the libraries:

* [D3](http://d3js.org/) - The king of visualization online. Popular, very well-designed, svg-based.
* [Highcharts](http://www.highcharts.com/) - Popular, feature-rich, svg-based, commercial.
* [Dygraphs](http://dygraphs.com/) - Canvas-based, mature line chart library, the code is a bit soupy but well tested.
* [Rickshaw](http://code.shutterstock.com/rickshaw/) - A sugar layer on top of D3 for reusable time series charts.
* [Chart.js](http://www.chartjs.org/) - I think I'm missing something with this framework (because it's so popular for being so young), but it seems very poorly designed.
* [Plain Canvas](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D) - Native browser API.

## Streaming Line Charts
Minimal configuration, no axis or grid lines, attempting to redraw as fast as possible (setTimeout(draw, 0)) with one data pushed and one data shifted out with each draw (1,000 points to draw are maintained at all times).

* [D3](http://ozan.io/charting-library-comparison/d3/streaming-line-chart.html) - Surprisingly fast (as fast as native canvas), quite a bit more scripting required though (as opposed to passing in config params to the libraries below).
* [Highcharts](http://ozan.io/charting-library-comparison/highcharts/streaming-line-chart.html) - Huge number of options made it difficult to just get the line with nothing else, runs sloooowww.
* [Dygraphs](http://ozan.io/charting-library-comparison/dygraphs/streaming-line-chart.html) - Fairly fast, the api is a bit weird in updates in that it's very "file" centric, which doesn't lend itself very well to streaming data.
* [Rickshaw](http://ozan.io/charting-library-comparison/rickshaw/streaming-line-chart.html) - Oddly buggy (clipping at top and bottom) and slow for being a thin layer on top of D3.
* [Chart.js](http://ozan.io/charting-library-comparison/chartjs/streaming-line-chart.html) - I think I'm missing something with this framework (because it's so popular for being so young), but this library seems very poorly designed. For example, every data point in the chart requires a label (so if you have 1000 data points, you need 1000 labels).
* [Plain Canvas](http://ozan.io/charting-library-comparison/custom/streaming-line-chart.html) - Baseline benchmark.
