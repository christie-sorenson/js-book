# ZingChart
Here I will test zingchart

{% chart %}
{
    // NOT need to specified `bindto` here
    data: {
        type: 'bar',
        columns: [
            ['data1', 30, 200, 100, 400, 150, 250],
            ['data2', 50, 20, 10, 40, 15, 25]
        ],
        axes: {
            data2: 'y2'
        }
    },
    axis: {
        y2: {
            show: true
        }
    }
}
{% endchart %}

{% zingchart width=300, height=300 %}
{
    "type":"bar",  
    "series":[  
        { "values": [35, 42, 67, 89]},
        { "values": [28, 40, 39, 36]}
    ]
}
{% endzingchart %}
