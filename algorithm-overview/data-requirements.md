# Data Requirements

Arcos is aimed at analysing time series data which should be arranged in [long format](https://en.wikipedia.org/wiki/Wide_and_narrow_data#Narrow). Each row should define the object’s location, time, and optionally the measurement value. For the implementations in R and python, the objects don't necessarily need to be tracked over time. However, it is recommended as it allows a more in-depth downstream analysis of ARCOS's output.

An example dataset could look like this:

<table><thead><tr><th>Index</th><th width="150">t</th><th width="150">x</th><th width="150">y</th><th width="150">m</th><th width="150">id</th><th>Position</th></tr></thead><tbody><tr><td>0</td><td>1</td><td>0.22</td><td>-0.15</td><td>0</td><td>1</td><td>0</td></tr><tr><td>1</td><td>1</td><td>0.88</td><td>-0.11</td><td>0</td><td>2</td><td>0</td></tr><tr><td>2</td><td>1</td><td>1.93</td><td>0.07</td><td>0</td><td>3</td><td>0</td></tr><tr><td>3</td><td>1</td><td>2.95</td><td>0.18</td><td>0</td><td>4</td><td>0</td></tr><tr><td>4</td><td>1</td><td>3.90</td><td>-0.04</td><td>0</td><td>5</td><td>0</td></tr></tbody></table>

For the napari-plugin, as of now, a track id is required.
