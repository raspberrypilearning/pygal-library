The pygal library allows you to create interactive charts from data.

```python
from pygal import *
```

To create a chart with pygal, you need to use one of the functions provided by the library:
 - `Bar()` will create a bar or column chart
 - `Pie()` will create a pie chart

```python
chart = Pie()
```

You then need to add some data to the chart using the `add()` function of your chart:

```python
chart.add(item, value)
```

Where:
 - `item` is a string — it might be a country, a person, a type of car, etc.
 - `value` is the number you want to display related to `item`

Finally, you need to call the `render()` function of your chart to display it.

For example:

```python
from pygal import Pie
# Create a Pie chart
chart = Pie()
# Add some data
chart.add('Cats', 5)
chart.add('Dogs', 10)
chart.add('Rabbits', 10)
# Display the chart
chart.render()
```

![A pie chart, displaying progressively larger sections for cats, dogs, and rabbits](images/pie.png)

