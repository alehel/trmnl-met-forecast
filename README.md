# Met.no Weather Forecast for TRMNL

A weather forecast plugin for [TRMNL](https://usetrmnl.com) e-paper screens that displays current and upcoming weather conditions using data from The Norwegian Meteorological Institute ([met.no](https://www.met.no)). Only the full-screen layout is provided, designed for the TRMNL X (1040×780); on smaller screens it shows an "only supported on TRMNL X" notice instead.

## Screenshots

Summer afternoon (English) — current conditions with UV and sunscreen window, today hour by hour with the current hour highlighted, tomorrow in 2-hour steps, then 6-hour blocks:

![Full layout, summer afternoon, English](screenshots/full-summer-en.png)

Winter night (Norwegian) — negative temperatures, max/min ranges in the 6-hour blocks, no sunscreen window:

![Full layout, winter night, Norwegian](screenshots/full-winter-no.png)

*The previews are rendered with placeholder weather glyphs; on the device the plugin uses TRMNL's hosted weather icon set.*

**Features:**
- **Current Conditions Panel**: Large weather icon with temperature, "feels like" temperature (wind chill/heat index), wind speed and direction, precipitation, humidity, pressure, and cloud cover
- **UV & Sunscreen Window**: Current clear-sky UV index and the time range when UV is forecast to be 3 or higher — i.e. when sunscreen is recommended (rolls over to tomorrow's window in the evening)
- **Hour-by-hour Timeline**: Today always shows all 24 hours — past hours as dimmed placeholders (the met.no forecast API carries no past data) and the current hour highlighted — followed by tomorrow in 2-hour rows (precipitation summed, temperature averaged) and 6-hour blocks with max/min temperatures for the two days after, with day headers and dates at each day change
- **Configurable Location**: Set custom latitude and longitude coordinates for any location
- **Multi-language Support**: Available in English and Norwegian

**Location:** `/met-no/`

## Credits

This project is based on [argoroots/trmnl](https://github.com/argoroots/trmnl) by [Argo Roots](https://github.com/argoroots), whose met.no plugin provided the original layouts, weather symbol mapping, and translations. The TRMNL X full-screen redesign, UV/sunscreen section, and aggregation logic were built on top of that foundation. The original work is MIT licensed, and this repository retains its license.
