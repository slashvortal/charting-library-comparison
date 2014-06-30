# Charting Library Comparison

Currently this is a benchmarking tool for streaming line charting using various
libraries. Each link points to a minimal configuration of the library attempting to
draw streaming data as fast as possible (maintaining 1000 points at all times. 
The ops/second are logged to the console.

* [D3](http://ozan.io/charting-library-comparison/d3/) - Popular, well-designed, svg-based.
* [Highcharts](http://ozan.io/charting-library-comparison/highcharts/) - Popular, feature-rich, svg-based, slow.
* [Dygraphs](http://ozan.io/charting-library-comparison/dygraphs/) - Canvas-based, over 5 years old, code is a bit soupy but seems well tested.
* [Rickshaw](http://ozan.io/charting-library-comparison/rickshaw/) - A sugar layer on top of D3 to enable reusable charts.
* [Chart.js](http://ozan.io/charting-library-comparison/chartjs/) - I think I'm missing something with this framework (because it's so popular for being so young), but it seems very poorly designed.
* [Plain Canvas](http://ozan.io/charting-library-comparison/custom/) - Baseline benchmark drawing lines directly to canvas