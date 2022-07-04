# Data Requirements

Arcos is aimed at analysing time series data which should be arranged in [long format](https://en.wikipedia.org/wiki/Wide\_and\_narrow\_data#Narrow). Each row should define the object’s location, time, and optionally the measurement value. For the implementations in R and python, the objects don't necessarily need to be tracked over time. However, it is recommended as it allows a more in-depth downstream analysis of ARCOS's output.

An example dataset could look like this:

| Index | t | x    | y     | m | id | Position |
| ----- | - | ---- | ----- | - | -- | -------- |
| 0     | 1 | 0.22 | -0.15 | 0 | 1  | 0        |
| 1     | 1 | 0.88 | -0.11 | 0 | 2  | 0        |
| 2     | 1 | 1.93 | 0.07  | 0 | 3  | 0        |
| 3     | 1 | 2.95 | 0.18  | 0 | 4  | 0        |
| 4     | 1 | 3.90 | -0.04 | 0 | 5  | 0        |

For the napari-plugin, as of now, a track id is required.
