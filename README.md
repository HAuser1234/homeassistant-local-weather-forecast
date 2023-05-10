# Homeassistant 12h local weather forecast. ~94% accurate*

this homeassistant integration creates sensors to forecast local weather without the need for external services.
Therefore it helps to get accurate weather data for the next 12h without the problem of changing services, API's ...
Also only a barometer as a sensor is required (can also be pulled from online). But the forecast can be made more accurate with more sensors.


# Features
* 2 Forcaster Models (zambretti + Negretti and Zambra)
* rain probability
* approximate timestamps for weather change (at reboot it can take some time for them to be accurate!)
* text prognosis
* simple temperature forecast
* extract general weather conditions
* full english an german support

# card
English and german version:

![grafik](https://github.com/HAuser1234/homeassistant-local-weather-forecast/assets/122117318/660ae494-a364-4fcb-8fff-5f8b31890c21)
![grafik](https://github.com/HAuser1234/homeassistant-local-weather-forecast/assets/122117318/30a135b7-ed0a-4cd2-a9fd-9d0b75570df8)



# Installation
please contribute ANY upgrades to the card or algorythm thia helps everybody!
* copy weather_forecast.yaml into your custom yaml integrations folder
* make changes for your individual setup (edit settings marked in weather_forecast.yaml
* copy the card as a manual yaml config into lovelace. !mushroom required, vertical-stack-in-card required!
* edit the current production of solar entity in the conditional cards

# sources
https://github.com/sassoftware/iot-zambretti-weather-forcasting
https://integritext.net/DrKFS/zambretti.htm
https://www.mikrocontroller.net/topic/385242
http://www.beteljuice.co.uk/zambretti/forecast.html

* according to https://github.com/sassoftware/iot-zambretti-weather-forcasting
_

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.

