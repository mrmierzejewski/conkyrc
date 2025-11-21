Conky configuration file
========================

These are my Conky configuration files.

![Conky](https://raw.github.com/zenzire/conkyrc/master/screenshot.png)


Installation
------------

Fetch the configuration files from the GitHub repository:

``
$ git clone git://github.com/mrmierzejewski/conkyrc.git ~/.conky
``

Create link:

``
ln -s ~/.conky/conkyrc ~/.conkyrc
``

Enjoy!

Features
--------

* weather with forecast
* CPU graph
* memory graph
* network graph
* processes 

Weather Configuration
---------------------

This configuration uses OpenWeatherMap API (Yahoo Weather API was retired in 2019).

To configure weather:

1. Get a free API key from https://openweathermap.org/api
   - Sign up for a free account
   - Navigate to API keys section
   - Copy your API key

2. Edit `conkyrc` and replace:
   - `YOUR_API_KEY` with your OpenWeatherMap API key
   - `YOUR_LOCATION` with your location (e.g., "London,UK", "New York,US", or coordinates like "40.7128,-74.0060")

3. Location format options:
   - City name: "London"
   - City with country: "London,UK"
   - Coordinates: "40.7128,-74.0060"

