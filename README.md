# Timeseries regression model
The premise of this timeseries regression model for building sensor data, is given some combination of readings from 1 or more sensors,
how accurately can we forecast the anticipated output of any one other sensor with the assumption of a naturally causal relationship
between atmospheric condition measurements being used. Example use case would be in regards to sensor maintenance and the ability to
use the model to determine if there are possible device malfunctions indicating that service or replacement is needed. Secondary use
case example would be pattern detection to monitor general building activity & and any inexplicable deviations from normal patterns.

This notebook uses the data for room 413 as an example test case. Production functionality would involve periodic cycles for any number
of rooms simultaneously. Also the end goal will be to display this model as a streamlit webapp once the code is adjusted to the streamlit
file format. Stay tuned.

# About Dataset
## Context
**source: https://www.kaggle.com/datasets/ranakrc/smart-building-system**

This dataset is collected from 255 sensor time series, instrumented in 51 rooms in 4 floors of the Sutardja Dai Hall(SDH) at UC Berkeley. It can be used to investigate patterns in physical properties of a room in a building. Moreover, it can also be used for experiments relating to Internet-of-Things (IoT), sensor fusion network or time-series tasks. This dataset is suitable for both supervised (classification and regression) and unsupervised learning (clustering) tasks.
Content

Each room includes 5 types of measurements: CO2 concentration, room air humidity, room temperature, luminosity, and PIR motion sensor data, collected over a period of one week from Friday, August 23, 2013 to Saturday, August 31, 2013. The PIR motion sensor is sampled once every 10 seconds and the remaining sensors are sampled once every 5 seconds. Each file contains the timestamps (in Unix Epoch Time) and actual readings from the sensor.

The passive infrared sensor (PIR sensor) is an electronic sensor that measures infrared (IR) light radiating from objects in its field of view, which measures the occupancy in a room. Approximately 6% of the PIR data is non-zero, indicating an occupied status of the room. The remaining 94% of the PIR data is zero, indicating an empty room.
Acknowledgements

If you use the dataset, please consider citing the following paper:
Dezhi Hong, Quanquan Gu, Kamin Whitehouse. High-dimensional Time Series Clustering via Cross-Predictability. In AISTATS'17.

