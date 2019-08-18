# Drawing with Data
This chapter talks about making bar charts and scatter plots

## Notes
- SVG coordinates are from the top left corner
- The enter() method iterates over the data
- Make vizualizations scalable based on the dataset using `dataset.length`

Example 
```javascript
var w = 500
var h = 200
var svg = d3.select("body")
            .append("svg")
            .attr("width", w)
            .attr("height", h);

        svg.selectAll("circle")
            .data(dataset)
            .enter()
            .append("circle")
            .attr("cx", function (d) {
                return d[0];
            })
```