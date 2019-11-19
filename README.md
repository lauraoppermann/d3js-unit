# D3js-Unit for VisuEngine

This Unit can be used for [VisuEngine](https://github.com/lauraoppermann/VisuEngineClone). It is based on [D3.js](https://d3js.org/).

## What to mind when using Cluster Visualization
The EJS files clusteringImage, clusteringLiveStreaming and clusteringVideo allow you to build clustering visualizations with or without animation.

### Example chart 
![ExampleGraph2](https://user-images.githubusercontent.com/50273734/68613980-3bb26380-04c0-11ea-8ab9-0633b0cfd937.PNG)

### What parameters to set for cluster visualization

|parameter 		|meaning   							|type 	|
|---			|---								|---	|
|title   		|sets a title for the chart					|string |
|height   		|defines the height in pixel of the chart			|number |
|width   		|defines the width in pixel of the chart			|number |
|maxX   		|defines the max number on the x axis				|number |
|minX   		|defines the min number on the x axis				|number |
|maxY   		|defines the max number on the y axis				|number |
|minY   		|defines the min number on the y axis				|number |
|pointColor   		|sets the datapoints to given color (valid css colors)		|string |
|clusterColor   	|sets the cluster to given color (valid css colors)		|string |
|yLabel   		|defines label for y axis					|string |    
|xLabel   		|defines label for x axis					|string |
|dataRefreshInterval   	|defines the interval in which the chart will be rerendered	|number |
|visibleDataPointsLimit |defines how many datapoints will be shown in the chart		|number |
|data   		|contains the data (datapoints and cluster)			|object | 

### Format of the data parameter

```
data: {
    points: [
       {
            x: 11.3,
            y: 23.2, 
            timeStamp: "t1 Zeitstempel fuer diesen Punkt"
        },
        {
            x: 3.3,
            y: 53.2, 
            timeStamp: "t2 Zeitstempel fuer diesen Punkt"
        }
    ],
     cluster: {
        t1: [
            {
                x: 15.3,
                y: 13.2, 
                radius: 5.0,
            },
            {
                x: 5.3,
                y: 43.2, 
                radius: 2.3,
            }
        ]
    }
}
```
