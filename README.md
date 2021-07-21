# WeatherPy
PyWeather was created to help find cities across the world and gather weather data. This can be used or tweaked to find other weather data, have more or less cities, change latitude and longitude ranges, and much more. 

## Information
As written, PyWeather will find 2000 latitude and longitude combinations and run them through the citipy python library. With the .nearest_city().city_name() function we can convert Latitude and Longitude to city names. After generating a unique list of city names, we can run them through the [OpenWeather API](https://openweathermap.org/api). The specific API utilized here is "Current Weather Data". While reviewing data keep in mind that this will not capture the full picture of weather conditions due to the inability to caputre time sensitive events(Think seasons or weather cycles like hurricanes). With this data we can then create all kinds of charts to visualize the data.

## Prerequisites
For best perfomance please install [citipy](https://github.com/wingchen/citipy). This can be done by using terminal and running `pip install citipy`. For the best experience please make sure the following is installed as well.
* jupyterlab v3.0.16

### Setting up API keys
We will also want to make sure that you create a file for your api keys. You will need two independent keys for this to work.
1. Clone repository
2. Navigate to repository and create identical files named "api_keys.py" in both folders:
    * WeatherPy
    * VacationPy
3. Copy the file contents below and edit with your api keys. 
    * Line 1: weather_api_key = "YourAPIKey"
    * Line 2: g_key = "YourAPIKey
4. If you do not have an API key, you can get them here:
    * [Google Cloud API](https://console.cloud.google.com/google/maps-apis/)
    * [OpenWeather API](https://openweathermap.org/api)
 
 
 You should now be ready to roll.
 
