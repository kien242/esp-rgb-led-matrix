# PIXELIX
![PIXELIX](./images/LogoBlack.png)

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://choosealicense.com/licenses/mit/)

- [PIXELIX](#pixelix)
- [Plugins](#plugins)
- [Generic plugins](#generic-plugins)
  - [IconTextPlugin](#icontextplugin)
  - [IconTextLampPlugin](#icontextlampplugin)
  - [JustTextPlugin](#justtextplugin)
- [Dedicated plugins](#dedicated-plugins)
  - [BTCQuotePlugin](#btcquoteplugin)
  - [CountdownPlugin](#countdownplugin)
  - [DatePlugin](#dateplugin)
  - [DateTimePlugin](#datetimeplugin)
  - [FirePlugin](#fireplugin)
  - [GameOfLifePlugin](#gameoflifeplugin)
  - [GruenbeckPlugin](#gruenbeckplugin)
  - [OpenWeatherPlugin](#openweatherplugin)
  - [RainbowPlugin](#rainbowplugin)
  - [SensorPlugin](#sensorplugin)
  - [ShellyPlugSPlugin](#shellyplugsplugin)
  - [SunrisePlugin](#sunriseplugin)
  - [SysMsgPlugin](#sysmsgplugin)
  - [TempHumidPlugin](#temphumidplugin)
  - [TestPlugin](#testplugin)
  - [TimePlugin](#timeplugin)
  - [VolumioPlugin](#volumioplugin)
  - [WifiStatusPlugin](#wifistatusplugin)

# Plugins
The content of the display can be configured by installing an individual set of plugins.
Each plugin is identified by its unique UID.

There are two types of plugins available at the moment:
* [Generic plugins](#Generic-plugins)
* [Dedicated plugins](#Dedicated-plugins)

# Generic plugins
The generic plugins allow the user to control the different UI elements described in the plugin name via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix).

## IconTextPlugin
The IconTextPlugin shows an icon on left side, text on right side.\
Each part can be set separately via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/IconTextPlugin)

## IconTextLampPlugin
The IconTextLampPlugin shows an icon on left side, text on right side and lamps at the bottom.\
Each part can be set separately via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/IconTextLampPlugin).

## JustTextPlugin
The JustTextPlugin shows only text on the whole display.\
The text to be displayed can be set via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/JustTextPlugin)

# Dedicated plugins
Dedicated plugins are plugins which only serves one single purpose thy are only internaly cofigurable.

## BTCQuotePlugin
The BTCQuotePlugin shows the current exchange rate from Bitcoin to USD.\
Powered by [CoinDesk](https://www.coindesk.com/price/bitcoin)
 
## CountdownPlugin
The CountdownPlugin shows the remaining days until a configured target date.\
Target date and the description of the target day (plural/singular form) can be set via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/CountdownPlugin).

## DatePlugin
The DatePlugin shows the current date. At the bottom the day of the week is shown, starting from the left with Monday.

## DateTimePlugin
The DateTimePlugin shows the current time and date. First the time is shown for half of the slot duration and after it the date. At the bottom the day of the week is shown, starting from the left with Monday.

## FirePlugin
The FirePlugin shows a animated fire on the display.

## GameOfLifePlugin
The GameOfLifePlugin shows the game of life game on the display.

## GruenbeckPlugin
The GruenbeckPlugin shows the remaining system capacity (parameter = D_Y_10_1 ) of the Gruenbeck softliQ SC18 via the system's RESTful webservice.\
The IP address of the Gruenbeck webserver can be set via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/GruenbeckPlugin).

## OpenWeatherPlugin
The OpenWeatherPlugin shows the current weather condition (icon and temperature) and one aditional information (uvIndex, humidity or windspeed) .\
Information provided by [OpenWeather](https://openweathermap.org/).\
In order to use the plugin an API key is necessary, see https://openweathermap.org/appid for further information.\
The coordinates (latitude & longitude) of your location, your API key and the desired additional information to be displayed can be set via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/OpenWeatherPlugin).

## RainbowPlugin
The RainbowPlugin shows an animated rainbow on the display.

## SensorPlugin
The plugin shows sensor values of the selected sensor channel.

## ShellyPlugSPlugin
The ShellyPlugSPlugin shows the current AC power being drawn via a Shelly PlugS, in watts.\
The IP address of the Shelly PlugS webserver can be set via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/ShellyPlugSPlugin).

## SunrisePlugin
The SunrisePlugin shows the current sunrise / sunset times for a configured location.\
The coordinates (latitude & longitude) of your location can be set via the [REST API](REST.md#endpoint-base-uridisplayuidplugin-uidlocation).\
Powered by sunrise-sunset.org

## SysMsgPlugin
The SysMsgPlugin is a system plugin, which is used to splash important informtions to the user. Note, it can not be uninstalled.

## TempHumidPlugin
Th TempHumidPlugin displays the temperature (in °C) and Humidity (in %) based on the readings of sensor connected to Pixelix.

## TestPlugin
The TestPlugin can be used to check whether the LED matrix topology (layout) is correct or not.

## TimePlugin
The TimePlugin shows the current time.

## VolumioPlugin
The VolumioPlugin shows the current VOLUMIO state as icon and the played artist/title.\
If the VOLUMIO server is offline, the plugin gets automatically disabled, otherwise enabled.\
The host address of the Volumio webserver can be set via the [REST API](https://app.swaggerhub.com/apis/BlueAndi/Pixelix/1.1.0#/VolumioPlugin).

## WifiStatusPlugin
The WifiStatusPlugin shows the current wireless signal strength.