# Manual

Retrieve weather data for a city. Usage is as simple as it gets. Just provide a city name (and country for clarification) in *Drafts* and trigger the action.

For example, this will get current weather data for Darmstadt in Germany:

    darmstadt, germany
	
The result will be pushed to *Drafts*. It will look like this:

    Weather in Darmstadt
    Latitude: 49.87056
    Longitude: 8.64944
    ====================
    Temperature: 23°C Sky is clear
    Clouds: 0%
    Humidity: 38%
    Sunrise: 2013-09-02 06:43:10
    Sunset: 2013-09-02 20:06:33
    	
    Data provided by www.openweathermap.org
	
That's it.

# Remarks

- Weather data provided by [Open Weather Map](http://openweathermap.org).
- There is one option variable in the script: UNITS. If left an empty string, the output will show temperatures in Fahrenheit. Otherwise ***&units=metric*** will use the metric system.
