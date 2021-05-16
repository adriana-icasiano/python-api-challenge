# python-api-challenge
## Table of Contents ##
* [WeatherPy (Part 1)- Assignment Requirement](https://github.com/adriana-icasiano/python-api-challenge#WeatherPy-Requiremnet)
* [WeatherPy - Solution](https://github.com/adriana-icasiano/python-api-challenge#WeatherPy-Solution)
* [Observation 1](https://github.com/adriana-icasiano/python-api-challenge#Observation-1.)
* [Observation 2](https://github.com/adriana-icasiano/python-api-challenge#Observation-2.)
* [Observation 3](https://github.com/adriana-icasiano/python-api-challenge#Observation-3.)
* [VacationPy (Part 2)- Assignment Requirement](https://github.com/adriana-icasiano/python-api-challenge#VacationPy-Requirement)
* [VacationPy - Solution](https://github.com/adriana-icasiano/python-api-challenge#VacationPy-Solution)

## WeatherPy Requirement
Students are tasked creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, students would be utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api) to create a representative model of weather across world cities. Information collected from Open Weather Map API include latitude, longitude, windspeed, cloudiness, humidity, and country for each of the 500+ cities.

## VacationPy Requirement
Using the data generated in WeatherPy, students are tasked with generating a HeatMap using Google Maps to visualize the intensity of humidity in each of the 500+ cities. Further, students will narrow the cities down based on ideal weather conditions for vacationing, and then using GoogleMap Nearby Search API to identify hotels within 5,000 meters of the city location. A marker with hotel name will be created on the heat map for each hotel.

## WeatherPy Solution
# Temperature
## Observation 1. 
The closer a city is from the equator, the higher the temperature. Higher negative latitude means further south of the equator. From the plot, the most negative latitude has the lowest temperature on the left side of the plot. As the latitude gets closed to zero (i.e. the equator) the temperature rises. As the latitude increase towards the right of the plot, or when the city is further from the equator, the temperature decreases. See further analysis below on Northern and Southern Hemisphere. 

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Temp.png)

## Northern Hemisphere Latitude vs. Max Temperature

The r-value is -0.8387276626376419. Therefore, latitude in the northern hemisphere has a strong negative relationship with the max temperature.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Max%20Temp%20N.Hem.png)

## Southern Hemisphere Latitude vs Max Temperature

The r-value is 0.7302547842043156. Therefore, latitude in the southern hemisphere has a strong positive relationship with the max temperature.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Max%20Temp%20S.Hem.png)

# Cloudiness
## Observation 2.
The plots are very scattered through out. Cloudiness is impacted by the altitudes not latitudes. The plot which shows no obvious relationship between latitude and cloudiness is consistent with this basic understanding. See further analysis below on Northern and Southern Hemisphere. 

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Cloudiness.png)

## Northern Hemisphere Latitude vs. Cloudiness

The r-value is 0.1029201140767342 Therefore, latitude in the northern hemisphere has a weak positive relationship with cloudiness.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Cloudiness%20(%25)%20N.Hem.png)

## Southern Hemisphere Latitude vs Cloudiness

The r-value is 0.07783404768292017. Therefore, latitude in the southern hemisphere has a weak positive relationship with cloudiness.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Cloudiness%20S.Hem.png)

# Humidity
## Observation 3.
The humidity appears to be higher near the equator (latitude = zero). According to ![UCAR Center of Science Educatiion](https://scied.ucar.edu/learning-zone/how-weather-works/humidity), warm air holds more water. While the relationship doesn't seem to be strong, there appears to be a slight relationship between latitude at humidity. See further analysis below on Northern and Southern Hemisphere. 

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Humidity.png)

## Northern Hemisphere Latitude vs. Humidity

The r-value is 0.01956017005962567. Therefore, there is a weak positive relationship between the latitude and humidity in the northern hemisphere.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Humidity%20N.Hem.png)

## Southern Hemisphere Latitude vs Humidity

The r-value is 0.16741607242655293. Therefore, there is a weak positive relationship between the latitude and humidity in the southern hemisphere.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Humidity%20(%25)%20S.Hem.png)

# Wind Speed
The plots are very scattered through out the plot. It appears that latitude does not have a relationship with wind speed.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Wind%20Speed.png)

## Northern Hemisphere Latitude vs. Wind Speed

The r-value is -0.0032295720403230834. Therefore, there is a weak positive relationship between the latitude and wind speed in the northern hemisphere.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Wind%20Speed%20N.Hem.png)

## Southern Hemisphere Latitude vs Wind Speed

The r-value is -0.1721991016726608. Therefore, there is a weak negative relationship between the latitude and wind speed in the southern hemisphere.

![](https://github.com/adriana-icasiano/python-api-challenge/blob/578eac3e6c96d8ba33f74ac9cda00fa4db3da860/WeatherPy/Images/Lat%20vs%20Wind%20Speed%20S.Hem.png)

## VacationPy Solution
## Heat Map of Intensity of Humidity of 600 cities

![](https://github.com/adriana-icasiano/python-api-challenge/blob/4f110cb37ca5d24fa9d19d7b0e3a1f09c31d5f1a/VacationPy/Images/HeatMap1.PNG)

## Heat Map of Intensity of Humidity with Hotel Markers

![](https://github.com/adriana-icasiano/python-api-challenge/blob/2deb1d3a08fe7502f54fff7386d20b015749b2b2/VacationPy/Images/HeatMap%20Hotel%20Markers.PNG)
