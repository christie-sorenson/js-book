# ZingChart


{% zingchart src='./zingchart.json' width=700 height=200 %}

{% zingchart width=700, height=200 %}
{
  "graphset":[
{
 	type: "bar",
 	"width":"33%",
 	"height":"100%",
 	"x":"1%",
 	"y":"1%",
	series : [
		{
			values : [35,42,67,89],
			"bar-width":"10%"
		}
	]
},
{
 	type: "bar", 
 	"width":"33%",
 	"height":"100%",
 	"x":"34%",
 	"y":"1%",
	series : [
		{
			values : [35,42,67,89],
			"bar-width":"100%"
		}
	]
},
{
 	type: "bar",
 	"title":{
 	  "text":"Just Right"
 	  },
 	"width":"33%",
 	"height":"100%",
 	"x":"67%",
 	"y":"1%",
	series : [
		{
			values : [35,42,67,89],
			"bar-width":"80%"
		}
	]
}
]
}
{% endzingchart %}

{% zingchart width=700, height=700 %}
{
"graphset":[
    {
        "type":"mixed",
        "width":"70%",
        "background-color":"#454754",
        "title":{
            "y":"10px",
            "text-align":"left",
            "background-color":"none",
            "text":"SALES OVERVIEW",
            "font-weight":"normal",
            "font-family":"Arial",
            "font-color":"#ffffff",
            "font-size":"18px",
            "height":"40px",
            "padding-left":"20px"
        },
        "plotarea":{
            "margin":"75px 75px 5px 67px"
        },
        "scale-x":{
            "values":["J","F","M","A","M","J","J","A","S","O","N","D"],
            "flat":false,
            "line-color":"#55717c",
            "offset-y":"4px",
            "guide":{
                "visible":false
            },
            "label":{
                "font-size":"11px",
                "font-family":"Arial",
                "font-color":"#ffffff",
                "font-weight":"normal"
            },
            "item":{
                "tooltip":{
                    "text":"%months"
                },
                "font-size":"10px",
                "font-family":"Arial",
                "font-color":"#c0c0c0"
            },
            "tick":{
                "visible":false
            }
        },
        "scale-y":{
            "line-color":"none",
            "values":"0:100000:20000",
            "multiplier":true,
            "label":{
                "text":"Net Profit",
                "font-size":"11px",
                "font-family":"Arial",
                "font-color":"#ffffff",
                "font-weight":"normal"
            },
            "item":{
                "font-size":"10px",
                "font-family":"Arial",
                "font-color":"#c0c0c0"
            },
            "guide":{
                "line-style":"solid",
                "line-color":"#5e606c",
                "alpha":1
            },
            "tick":{
                "visible":false
            }
        },
        "scale-y-2":{
            "line-color":"none",
            "values":"0:500:100",
            "multiplier":true,
            "label":{
                "text":"Units Sold",
                "offset-x":"5px",
                "font-size":"11px",
                "font-family":"Arial",
                "font-color":"#ffffff",
                "font-weight":"normal"
            },
            "item":{
                "font-size":"10px",
                "font-family":"Arial",
                "font-color":"#c0c0c0"
            },
            "guide":{
                "visible":false
            },
            "tick":{
                "visible":false
            }
        },
        "plot":{
            
        },
        "series":[
            {
                "values":[48000,31000,62000,40500,44550,29500,46000,70050,39500,45800,29000,15000],
                "type":"bar",
                "background-color":"#6597a2",
                "hover-state":{
                    "visible":1,
                    "border-width":"4px",
                    "border-color":"#2f6672",
                    "alpha":0.5
                },
                "tooltip":{
                    "background-color":"#2f6672",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                },
                "animation":{
                    "delay":0,
                    "effect":4,
                    "speed":"1000",
                    "method":"0",
                    "sequence":"0"
                }
            },
            {
                "values":[110,58,104,357,294,367,285,340,397,425,254,187],
                "type":"line",
                "line-color":"#96feff",
                "line-width":2,
                "marker":{
                    "background-color":"#a3bcb8",
                    "border-width":2,
                    "shadow":0,
                    "border-color":"#88f5fa"
                },
                "tooltip":{
                    "background-color":"#54ced4",
                    "font-color":"#454754",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                },
                "animation":{
                    "delay":500,
                    "effect":5,
                    "speed":"1800",
                    "method":"0",
                    "sequence":"1"
                },
                "scales":"scale-x,scale-y-2"
            }
        ]
    },
    {
        "type":"pie",
        "width":"34%",
        "x":"66%",
        "background-color":"#454754",
        "title":{
            "background-color":"none",
            "font-weight":"normal",
            "font-family":"Arial",
            "font-color":"#ffffff",
            "height":"40px"
        },
        "plotarea":{
            "margin":"60px 10px 0px 0px"
        },
        "plot":{
            "value-box":{
                "visible":false
            },
            "animation":{
                "delay":0,
                "effect":2,
                "speed":"300",
                "method":"0",
                "sequence":"1"
            }
        },
        "series":[
            {
                "text":"Product 1",
                "values":[15],
                "background-color":"#57dce5",
                "border-color":"#454754",
                "border-width":"1px",
                "shadow":0,
                "tooltip":{
                    "background-color":"#54ced4",
                    "font-color":"#454754",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                }
            },
            {
                "text":"Product 2",
                "values":[18],
                "background-color":"#9688f7",
                "border-color":"#454754",
                "border-width":"1px",
                "shadow":0,
                "tooltip":{
                    "background-color":"#796bdd",
                    "font-color":"#ffffff",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                }
            },
            {
                "text":"Product 3",
                "values":[20],
                "background-color":"#b659b4",
                "border-color":"#454754",
                "border-width":"1px",
                "shadow":0,
                "tooltip":{
                    "background-color":"#a03f9c",
                    "font-color":"#ffffff",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                }
            },
            {
                "text":"Product 4",
                "values":[16],
                "background-color":"#3bbcfc",
                "border-color":"#454754",
                "border-width":"1px",
                "shadow":0,
                "tooltip":{
                    "background-color":"#1b9ede",
                    "font-color":"#ffffff",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                }
            },
            {
                "text":"Product 5",
                "values":[21],
                "background-color":"#6597a2",
                "border-color":"#454754",
                "border-width":"1px",
                "shadow":0,
                "tooltip":{
                    "background-color":"#2f6672",
                    "font-color":"#ffffff",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"5px 10px"
                }
            }
        ]
    },
    {
        "type":"bar",
        "width":"100%",
        "background-color":"#454754",
        "border-bottom":"8px solid #565867",
        "plot":{
            "bar-space":"10px",
            "animation":{
                "delay":0,
                "effect":4,
                "speed":"1000",
                "method":"0",
                "sequence":"0"
            }
        },
        "plotarea":{
            "margin":"45px 30px 40px 65px"
        },
        "scale-x":{
            "values":["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"],
            "line-color":"#55717c",
            "offset-y":"4px",
            "tick":{
                "size":"5px",
                "line-color":"#55717c",
                "line-width":"1px",
                "visible":false
            },
            "guide":{
                "visible":false
            },
            "item":{
                "font-size":"10px",
                "font-family":"Arial",
                "font-color":"#c0c0c0"
            }
        },
        "scale-y":{
            "line-color":"none",
            "values":"0:50000:10000",
            "multiplier":true,
            "guide":{
                "line-style":"solid",
                "line-color":"#5e606c",
                "alpha":1
            },
            "tick":{
                "visible":false
            },
            "label":{
                "text":"Sales by Employee",
                "offset-x":"-5px",
                "font-size":"11px",
                "font-family":"Arial",
                "font-color":"#ffffff",
                "font-weight":"normal"
            },
            "item":{
                "padding-left":"2px",
                "font-size":"10px",
                "font-family":"Arial",
                "font-color":"#c0c0c0"
            }
        },
        "series":[
            {
                "values":[31000,39500,24300,36000,38000,45500,28500,38000,21000,17000,24000,17500],
                "background-color":"#57dde8",
                "tooltip":{
                    "background-color":"#54ced4",
                    "font-color":"#454754",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"20px 80px",
                    "alpha":0.75,
                    "text":"For when you have more to say..."
                }
            },
            {
                "values":[11500,36750,7000,44500,11500,28450,42900,26750,13050,32600,12500,14300],
                "background-color":"#978af6",
                "tooltip":{
                    "background-color":"#796bdd",
                    "font-color":"#ffffff",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"20px 80px",
                    "alpha":0.75,
                    "text":"Go ahead, make my day..."
                }
            },
            {
                "values":[21500,29550,14500,16500,28450,35600,21550,18750,11600,7500,14750,16000],
                "background-color":"#b857b4",
                "tooltip":{
                    "background-color":"#a03f9c",
                    "font-color":"#ffffff",
                    "border-radius":"6px",
                    "shadow":false,
                    "padding":"20px 80px",
                    "alpha":0.75,
                    "text":"Insights go here!"
                }
            }
        ]
    }
]
}
{% endzingchart %}
