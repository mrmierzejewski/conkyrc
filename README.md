Conky configuration file
========================

These are my Conky configuration files.

![Conky](https://raw.github.com/zenzire/conkyrc/master/screenshot.png)

A sleek, minimalist Conky configuration that displays real-time system information and weather data on your desktop. Features live weather forecasts with OpenWeatherMap integration, system resource monitoring (CPU, memory, disk I/O), network statistics, and process tracking—all in a clean, transparent overlay that stays out of your way.


Requirements
------------

* Conky 1.10 or later (uses Lua-based configuration syntax)
* Lua 5.1 or later (for Conky 1.10+ compatibility)


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

**Note:** This configuration uses the modern Lua-based syntax (Conky 1.10+). If you're using an older version of Conky, you may need to upgrade or use a legacy configuration format.

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

Troubleshooting
---------------

**Syntax Errors:**
If you encounter syntax errors like "syntax error near 'yes'" or "loadstring" errors, ensure you're using Conky 1.10 or later. The configuration uses the modern Lua-based syntax.

**Check your Conky version:**
``
$ conky --version
``

**For older Conky versions (< 1.10):**
You'll need to upgrade Conky to use this configuration, or convert it back to the legacy format (not recommended as Yahoo Weather API is no longer available).

**Weather not displaying:**
- Verify your OpenWeatherMap API key is correct
- Check that your location string is properly formatted
- Ensure you have internet connectivity
- Check the cached weather files: `~/.cache/weather-current.json` and `~/.cache/weather-forecast.json`

