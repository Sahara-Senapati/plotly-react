React Plotly.js in JavaScript

Plotly.js is a high-level, open source, declarative library used for building various charts and other web interfaces. Plotly.js ships with over 40 chart types, including 3D charts, statistical graphs, and SVG maps.
We can use react-plotly.js to embed D3 charts in our React-powered web application. This React component takes the chart type, data, and styling as Plotly JSON in its data and layout props, then draws the chart using Plotly.js.

Any chart that we create with the Plotly library is equipped with features like zooming in, zooming out, panning, auto-scaling, etc. These features can be useful when we want to study charts with a large number of plotted points.

The attributes that is provided within a plotly component can be broadly divided into two categories. The first one is called traces, which are objects that are used to provide information about the data to be plotted on the graph.
The second category is layout, which provides different attributes that control all the other aspects of the chart like its title or annotations. 

Common parameters we have in a Plotly Component

graphDiv

The functions in react all create or modify a plot that is drawn into a <div> element on the page, commonly referred to as graphDiv or plotDiv. The first argument to each function on this page is a reference to this element, and it can be either a DOM node, , or a string.
  
data

The data to be plotted is described in an array usually called data, whose elements are trace objects of various types (e.g. scatter, bar etc) 

layout

The layout of the plot refers to the non-data-related visual attributes such as the title, annotations etc.

config

High-level configuration options for the plot, such as the scroll/zoom/hover behaviour, is described in an object usually called config. The difference between config and layout is that layout relates to the content of the plot, whereas config relates to the context in which the plot is being shown.

Plotly.newPlot(graphDiv, data, layout, config)

Examples of some of the basic charts that plotly provides:- Bar Graph, Scatter Plot, Horizontal Bar Chart, Pie Chart etc.

In this application, I have added different basic charts of plotly as links in App.js.
As the user clicks on the link he will be rendered to a new page that displays that particular Plotly chart.



