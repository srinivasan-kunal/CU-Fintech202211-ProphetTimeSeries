# Time Series Forecasting with Prophet 

In this program I used the `prophet` library (formerly known as `fbprophet`) to create time series forecasts.

## Technologies
There are two critical python libraries in this program- `prophet` & `hvplot`. Sometimes, installing the prophet library may cause issues on certain machines. As a work around the `main_program` was created using google-collab (https://colab.research.google.com/).    

---
## Installation Guide

The top of the code installs the critical libraries needed for the program in google-collab (https://colab.research.google.com/). 

```python
from IPython.display import clear_output

try:
  !pip install pystan
  !pip install prophet
  !pip install hvplot
  !pip install holoviews
except:
  print("Error installing prophet")
finally:
  clear_output()
  print("Prophet was successfully installed")
```

---

## Usage

When using google-collab to execute the code a critical step is to import the raw-csv data into the collab work environment.

The code to import raw files may be found in several places within the `main_program`.

```python
from google.colab import files
uploaded = files.upload()
```
The program creates heatmaps to review the data on various dimensions of time, in order to make initial assessments about the trends and seasonalities present in the data.

Later, the `prohpet()` library is used to generated prediction for the M/s Mercado's online search results and the projection for sales over 90 days.  

---

## Contributors


Kunal Srinivasan

---

## License

2022 edX Bootcamps 