# api_challenge
## Overview  
<hr>

Analysis of humidity, temperature, cloudiness, and precipitation data against latitude from over 1000 randomly selected global cities.  Cities were selected randomly via the citipy package and the weather data was from API calls to OpenWeather.  Analysis was performed and visualized through Pandas and Matplotlib.
<br>
<br>
After analyzing each city's weather, that output was filtered further and used to map out ideal vacation locations and their respective nearby hotels using gmaps and an associated API key.

<br>

## Technologies    
*  Python
*  Pandas
*  Matplotlib
*  Requests

<br>

## Setup and Installation  
1. Imports and environment:  
    *  Python 3.6+  
    *  pandas  
    *  matplotlib.pyplot
    *  numpy
    *  requests
    *  time
    *  citipy
1. Activate environment and clone the repo
1. Get free API key from [OpenWeatherMap](https://openweathermap.org/appid#signup) by creating an account.
        Add the key to `config.py`  
1. Start Jupyter Notebook within the environment from the repo
1. Run `WeatherPy.ipynb` within the starter_code folder.
2. For `VacationPy.ipynb` , additional imports are needed:
        `gmaps` and `os`
3. Run `VacationPy.ipynb` only after running `WeatherPy.ipynb` as the second notebook is reliant on data given by the first.

<br>

## Data Source  
Dataset generated within the notebook.  The cities used in this analysis were randomly selected through the `citypy` package.  The weather data was retrieved through  [OpenWeather API](https://openweathermap.org/api). A free API key is needed to use this service.

<br>

## Analysis  

**`Note:`** All analysis images can be found in the `output_data` folder.  Each time the notebook is run in it's entirety, the images are updated and replaced.  

1.  Each comparison plot is demonstrated with an attached analysis in the given notebook. 

1.  Below is an example image generated from the notebook.

<figure>

![OpenWeather API Requests](./output_data/Fig1.png)  
<figcaption>Fig.1 - Scatter Plot showing Temperature versus Latitude
</figcaption>
</figure>  

<br>

<br>
1. The second notebook in this repo, `VacationPy.ipynb` , filters down the given cities from `WeatherPy.ipynb` and produces the cities with the most ideal weather conditions as well as the closest hotels to each respective city. A heatmap image is given in screenshot form to show the results of this analysis in addition to the original notebook findings.
<figure>

![OpenWeather API Requests](./output_data/Screenshot%20(49).png)  
<figcaption>Heatmap with pop-up info for each Vacation-worthy city
</figcaption>
</figure>
