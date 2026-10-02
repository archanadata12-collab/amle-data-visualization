# Group Work: Visualisation Task

In this group work you will use three plotting libraries: [Matplotlib](https://matplotlib.org/index.html), [Seaborn](https://seaborn.pydata.org/) and [Plotly](https://plotly.com/python/). They are among the most widely used in Python. By making the same chart in all three, you get a first impression of their advantages, disadvantages and differences.

## Task

Each group makes **one type of plot**, and makes it **once in each of the three libraries**: three plots in total. The table below gives each group its plot type and dataset.

| Group | Plot | Dataset | File |
| ----- | ---- | ------- | ---- |
| 1 | Scatter plot | Seattle Weather | `data/seattle-weather.csv` |
| 2 | Line plot | Seattle Weather | `data/seattle-weather.csv` |
| 3 | Bar chart | Seattle Weather | `data/seattle-weather.csv` |
| 4 | Geographical map | US Airports | `data/airports.csv` |

> [!NOTE]
> Group 4: geographical maps work best in Plotly, so focus on Plotly for this task. If you have time at the end, try the other libraries too.

Build your plots in the [template notebook](02_exercise_template.ipynb). It already imports the libraries and shows an example of a good plot. The data files are in the `data` folder at the top of the repository, so from the notebook you load them with a path such as `pd.read_csv("../data/seattle-weather.csv")`.

At the end, your notebook should contain the code for your three plots and, under each library's section, a short explanation: what the plot shows, and how the library was to work with compared with the others. You will share your notebook with the other groups, so together the notebooks form a set of reference examples for the rest of the course.

If you have not set up the environment yet, follow the Setup section in the [README](../README.md) first.

## The Datasets

**Seattle Weather** has one row per day from 2012 to 2015:

| Column | Meaning | Unit |
| ------ | ------- | ---- |
| `date` | The day, stored as text such as `2012/01/01` | |
| `precipitation` | Rain or snow that fell that day | mm |
| `temp_max` | Highest temperature of the day | °C |
| `temp_min` | Lowest temperature of the day | °C |
| `weather` | The type of weather: drizzle, rain, sun, snow or fog | |

The dataset also has a `wind` column, which you do not need for this task.

**US Airports** has one row per airport, with its code (`iata`), `name`, `city`, `state`, `country`, and its position as `latitude` and `longitude` in degrees. Almost all of them are in the United States: 3,372 of the 3,376. The other four are in Thailand and the Pacific, so they fall outside a map limited to the US.

## What Makes a Plot Good

Whether a plot is appealing is partly a matter of taste, but always check these points:

* The title, labels and all other text are readable.
* Every axis label includes its unit.
* The colours still work for people with colour blindness.
* The plot is easy to understand. Do not overwhelm your audience with too much detail or decoration.
