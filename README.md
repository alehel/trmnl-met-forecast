# Met.no Weather Forecast for TRMNL

A weather forecast plugin for [TRMNL](https://usetrmnl.com) e-paper screens that displays current and upcoming weather conditions using data from The Norwegian Meteorological Institute ([met.no](https://www.met.no)).

**Features:**
- **Current Conditions Panel** (full layout, designed for TRMNL X): Large weather icon with temperature, "feels like" temperature (wind chill/heat index), wind speed and direction, precipitation, humidity, pressure, and cloud cover
- **UV & Sunscreen Window** (full layout): Current clear-sky UV index and the time range when UV is forecast to be 3 or higher — i.e. when sunscreen is recommended (rolls over to tomorrow's window in the evening)
- **Hour-by-hour Timeline** (full layout): Today always shows all 24 hours — past hours as dimmed placeholders (the met.no forecast API carries no past data) and the current hour highlighted — followed by tomorrow in 2-hour rows (precipitation summed, temperature averaged) and 6-hour blocks with max/min temperatures for the two days after, with day headers and dates at each day change
- **Multi-day Forecast**: Displays weather for today, tomorrow, and upcoming days
- **Weather Icons**: Visual weather symbols based on met.no weather codes
- **Configurable Location**: Set custom latitude and longitude coordinates for any location
- **Multi-language Support**: Available in Estonian, English, Norwegian, Finnish, and Swedish
- **Multiple Layouts**: Full, half horizontal, half vertical, and quadrant layout options
- **Detailed Metrics**: Temperature, wind speed, and precipitation amount for each forecast period

**Location:** `/met-no/`
