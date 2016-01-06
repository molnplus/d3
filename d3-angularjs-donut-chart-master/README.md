##D3 driven animated and reusable donut chart wrapper into AngularJS directive - [live demo](http://iuriistavnichuk.github.io/d3-angularjs-donut-chart/).

Since the data is retrieved from the external JSON file the developer does not need to worry about generating data within the program. This makes the module more flexible and maintainable so this approach allows us to place uncountable amount of these charts on the page in the neat way without polluting your HTML.

### How to install
 + Copy `donutChart.js` wherever you want
 + Reference it in your index.html file
 + Reference the module in your app file :
     angular.module('MainWebApp', ['donutChart'])

### How to use
A donut chart is called using this syntax :

```html
<donut-chart path-to-json = "'json/donut-chart.json'"></donut-chart>
```

The pie chart directive attribute : `path-to-json`.


#### path-to-json
Your data must be JSON object.
```js
{
    "Results":
        [
            {"Title":"Funds Received",
                "CurrencySymbol":"$",
                "Amount":106.52,
                "TotalAmount":400,
                "CurrencyAbbreviation":"USD",
                "Unit":null,
                "TimeInterval":"/month"
            }
        ]
}
```
