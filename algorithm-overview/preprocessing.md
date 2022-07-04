# Preprocessing

### How to get the necessary input data for ARCOS

To get from raw data to data that ARCOS accepts as input, several different tools can be used. The steps neccessary can be summarised as follows:

1. Acquire your image data.
2. Segment images to identify individual objects.&#x20;
   * Tools that can be used for this purpose include Ilastik (a more general approach), simple image thresholding, or more specialised tools such as stardist, and cellpose in the case of microscopy data and many others.
3. Optionally, extract a measurement value from objects, for example from a fluorescent biosensor, other intensity changes, shape changes or something else entirely. This is needed if some objects should be excluded from the analysis based on a activity threshold.
4. Optionally, track detected objects across time and space. This is needed from subsequent downstream analysis but not necessarily for ARCOS itself.

### How to prepare the data with ARCOS

#### **Interpolate Measurments**

If the measurement column contains missing values, in the first step the data should be interpolated. Helper functions are available across all implementations.&#x20;

#### **Detrend and rescale the measurement**

Often time-series data can exhibit local and global trends that are introduced as artefacts of the data acquisition. In the case of fluorescence microscopy bleaching can be an example of such a bias. To help with this several de-trending methods are implemented in ARCOS, all of which are optional. There are three options available: \['none', 'lm', 'runmed']. With "none", the data is first rescaled to a feature range of 0,1. Subsequently, a short-term median filter is applied to the time series to reduce noise in the data. "lm" uses linear regression to detect long-term trends. Additionally, a short-term median filter is used to reduce noise in the time series. With "runmed", a long-term and a short-term median filter is used. After de-trending the data with options "lm" and "runmed", the output is rescaled to a feature range of 0,1.&#x20;

#### Binarization

ARCOS requires binarized data to detect and track collective event clusters. Binarization is done by setting a threshold and defining measurements below this threshold as 0 and above as 1. Alternatively, all input objects can be defined as "active" if no measurement is available.
