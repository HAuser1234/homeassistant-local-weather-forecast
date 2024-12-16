# Homeassistant 12h local weather forecast. ~94% accurate*
<a href="https://www.buymeacoffee.com/hauser1234" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>


<b> new Ecowitt integration released! use https://github.com/HAuser1234/HA_Ecowitt_Extended to direcly integrate your Ecowitt based weatherstation with this integration!</b>

This Home Assistant integration creates sensors to forecast local weather without the need for external services.
Therefore, it helps to get accurate weather data for the next 12h without the problem of changing services, API's, etc.
Only a barometer as a sensor is required (can also be pulled from online). But the forecast can be made more accurate with more sensors.
For me, the zambretti forecaster is pretty accurate, but you will have to monitor both models in order to find the better one for your location.

If you like this repository please leave a star ⭐


# Features
* 2 Forecast Models (Zambretti, and Negretti & Zambra)
  (you may have to change the card to use the other model, depending on which model is more accurate at your location)
* rain probability
* approximate timestamps for weather change (at reboot it can take some time for them to be accurate!)
* text prognosis
* simple temperature forecast
* extract general weather conditions
* full English and German support

# Sensors
Following sensors can be used:
* Barometer (required)
* Temperature (set value to 0 is missing) (optional)
* Wind speed (optional)
* Wind direction (optional)

# Card
English and German version:

![grafik](https://github.com/HAuser1234/homeassistant-local-weather-forecast/assets/122117318/3a4cb58b-617f-4a9a-8fb2-ec723a5b05c0)
![grafik](https://github.com/HAuser1234/homeassistant-local-weather-forecast/assets/122117318/19c8220a-4bfe-4a0f-a82a-c968cbfd5b31)


# Installation
Please contribute ANY upgrades to the card or algorithm - this helps everybody!
* copy weather_forecast.yaml into your custom yaml integrations folder
how to make a integrations folder:
1. add this to your configuration.yaml:

```
homeassistant:
  packages: !include_dir_named integrations
```
  
2. create a folder named 'integrations' in your config directory
3. copy weather_forecast.yaml in this folder

* make changes for your individual setup (edit settings marked in weather_forecast.yaml
* copy the card as a manual yaml config into lovelace. !mushroom required, vertical-stack-in-card required!
* edit the current production of solar entity in the conditional cards

# To-Do
* Improve algorithms
* Find bugs (please commit changes!)
* Make better temperature forecast
* Integrate maybe with a solar/battery-charge prediction tool: https://github.com/HAuser1234/Homeassistant-solar-forecast-charge-prediction

# sources
https://github.com/sassoftware/iot-zambretti-weather-forcasting
https://integritext.net/DrKFS/zambretti.htm
https://www.mikrocontroller.net/topic/385242
http://www.beteljuice.co.uk/zambretti/forecast.html

.* 94% according to https://github.com/sassoftware/iot-zambretti-weather-forcasting
_

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.

