# **Charts**

- Charts are better for displaying data. They're cleaner and much easier to read!

- Example:

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
`<meta charset="utf-8" />`
`<title>Chart.js demo</title>`
`<script src='Chart.min.js'></script>`
`</head>`
`<body>`
`</body>`
`</html>`

- Drawing a line chart: First thing you do is create a canvas element in HTML file.

- Example:

  `<canvas id="buyers" width="600" height="400"></canvas>`

- Next you'll need a script that will retrieve the context of the canvas!

- Example:

`<script>`
`var buyers = document.getElementById('buyers').getContext('2d');`
` new Chart(buyers).Line``(buyerData); `
`</script>`

- Inside the same line script tags we need to create out data plan, in this instance it's an object that contains labels for the base of our chart and datasets to describe the values on the chart.

- Example:

`var buyerData = {`
`labels : ["January","February","March","April","May","June"],`
`datasets : [`
`{`
`fillColor : "rgba(172,194,132,0.4)",`
`strokeColor : "#ACC26D",`
`pointColor : "#fff",`
`pointStrokeColor : "#9DB86D",`
`data : [203,156,99,251,305,247]`
`}`
`]`
`}`

> Drawing a pie chart:

* Example:

`<!DOCTYPE html>`
`<html lang="en">`
    `<head>`
        `<meta charset="utf-8" />`
        `<title>Chart.js demo</title>`
        `<!-- import plugin script -->`
        `<script src='Chart.min.js'></script>`
    `</head>`
    `<body>`
        `<!-- line chart canvas element -->`
        `<canvas id="buyers" width="600" height="400"></canvas>`
        `<!-- pie chart canvas element -->`
        `<canvas id="countries" width="600" height="400"></canvas>`
        `<!-- bar chart canvas element -->`
        `<canvas id="income" width="600" height="400"></canvas>`
        `<script>`
            `// line chart data`
            `var buyerData = {`
                `labels : ["January","February","March","April","May","June"],`
                `datasets : [`
                `{`
                    `fillColor : "rgba(172,194,132,0.4)",`
                    `strokeColor : "#ACC26D",`
                    `pointColor : "#fff",`
                    `pointStrokeColor : "#9DB86D",`
                    `data : [203,156,99,251,305,247]`
                `}`
            `]`
            `}`
            `// get line chart canvas`
            `var buyers = document.getElementById('buyers').getContext('2d');`
            `// draw line chart`
            `new Chart(buyers).Line(buyerData);`
            `// pie chart data`
            `var pieData = [`
                `{`
                    `value: 20,`
                    `color:"#878BB6"`
                `},`
                `{`
                    `value : 40,`
                    `color : "#4ACAB4"`
                `},`
                `{`
                    `value : 10,`
                    `color : "#FF8153"`
                `},`
                `{`
                    `value : 30,`
                    `color : "#FFEA88"`
                `}`
            `];`
            `// pie chart options`
            `var pieOptions = {`
                 `segmentShowStroke : false,`
                 `animateScale : true`
            `}`
            `// get pie chart canvas`
            `var countries= document.getElementById("countries").getContext("2d");`
            `// draw pie chart`
            `new Chart(countries).Pie(pieData, pieOptions);`
            `// bar chart data`
            `var barData = {`
                `labels : ["January","February","March","April","May","June"],`
                `datasets : [`
                    `{`
                        `fillColor : "#48A497",`
                        `strokeColor : "#48A4D1",`
                        `data : [456,479,324,569,702,600]`
                    `},`
                    `{`
                        `fillColor : "rgba(73,188,170,0.4)",`
                        `strokeColor : "rgba(72,174,209,0.4)",`
                        `data : [364,504,605,400,345,320]`
                    `}`
                `]`
            `}`
            `// get bar chart canvas`
            `var income = document.getElementById("income").getContext("2d");`
            `// draw bar chart`
            `new Chart(income).Bar(barData);`
        `</script>`
    `</body>`
`</html>`

> Basic usage

* At first sight a `<canvas>` looks like the `<img>` element, with the only clear differene being it doesn't have the *src* and **alt** attributes. Inded the `<canvas>` element has only two attributes, **width&height**. These are both optional and can also be set using the DOM properties. When no **width** and **height** attributes are specified, the canvas will initially be **300px** wide and **150px** high.