## Responsive Bar Charts with Bokeh, Flask and Anaconda with Python 3 

https://www.fullstackpython.com/blog/responsive-bar-charts-bokeh-flask-python-3.html


install environment:

	conda create -n responsiveChart


To activate this environment, use:

    source activate responsiveChart

To deactivate an active environment, use:

	source deactivate

install Bokeh and Flask and Pandasy:

	conda install bokeh flask pandas

---

small fix for chart.html:

    <!DOCTYPE html>
    <html>

    <head>
        <title>Bar charts with Bokeh!</title>
        <link href="http://cdn.pydata.org/bokeh/release/bokeh-0.12.6.min.css" rel="stylesheet">
        <link href="http://cdn.pydata.org/bokeh/release/bokeh-widgets-0.12.6.min.css" rel="stylesheet">
    </head>

    <body>
        <h1>Bugs found over the past {{ bars_count }} days</h1>
        {{ the_div|safe }}
        <script src="http://cdn.pydata.org/bokeh/release/bokeh-0.12.6.min.js"></script>
        <script src="http://cdn.pydata.org/bokeh/release/bokeh-widgets-0.12.6.min.js"></script>
        {{ the_script|safe }}
    </body>

    </html>
    
source on GitHub:

https://github.com/skidzo/rechart.git