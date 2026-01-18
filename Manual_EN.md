# FUSION IV - Complete Documentation

> ⚠️ **DISCLAIMER**: This repository contains user documentation only. No source code, algorithms, backend logic or licensing mechanisms are included. Any attempt to reverse engineer the product is prohibited.

![Version](https://img.shields.io/badge/version-Beta-blue)
![Platform](https://img.shields.io/badge/platform-Garmin%20Connect%20IQ-green)
![API](https://img.shields.io/badge/API-5.0.0%2B-orange)

---

## Table of Contents

1. [Overview](#overview)
2. [Compatibility](#compatibility)
3. [Main Features](#main-features)
4. [User Interface](#user-interface)
5. [Configuration](#configuration)
   - [System Settings](#system-settings)
   - [Display Settings](#display-settings)
   - [Data Fields](#data-fields)
   - [Color Customization](#color-customization)
   - [Weather](#weather)
6. [Available Data Types](#available-data-types)
7. [License and Activation](#license-and-activation)
8. [Installation](#installation)
9. [Support and Assistance](#support-and-assistance)

---

![FUSION IV Banner](docs/images/Banner.jpg)

---

## Overview

**FUSION IV** is a highly customizable watch face for Garmin Connect IQ watches. Designed to provide an optimal user experience, it combines modern design and functional richness with extensive customization of all on-screen elements.

### Key Features

- ✨ **Highly Customizable Interface**: 28 independently configurable colors
- 📊 **Multiple Data Fields**: 18 configurable data zones
- 🌦️ **Weather Integration**: Supports Garmin Weather and OpenWeatherMap
- ⚡ **Battery Optimization**: Intelligent power saving modes
- 🌍 **Multilingual Support**: 19 languages available
- 🎯 **Goals and Tracking**: Progress bars for your objectives
- 🌙 **Night Mode**: Configurable screen protection

---

## Compatibility

### Supported Watches

FUSION IV is compatible with the following Garmin watches:

#### Approach Series
- Approach S70 (42mm, 47mm)

#### Descent Series
- Descent Mk3 (43mm, 51mm)

#### Enduro Series
- Enduro 3

#### Epix Series
- Epix 2 (all variants)
- Epix 2 Pro (42mm, 47mm, 51mm)

#### Fenix Series
- Fenix 7 (all variants: standard, S, X, Pro)
- Fenix 7X Pro (with and without WiFi)
- Fenix 8 (43mm, 47mm, Pro 47mm, Solar 47mm/51mm)
- Fenix E

#### Forerunner Series
- Forerunner 265 (standard and S)
- Forerunner 570 (42mm, 47mm)
- Forerunner 955
- Forerunner 965
- Forerunner 970

#### MARQ Series
- MARQ 2 (all variants, including Aviator)

#### Venu Series
- Venu 3 (standard and S)
- Venu 4 (41mm, 45mm)

#### Vivoactive Series
- Vivoactive 6

#### Others
- D2 Mach 1

### System Requirements

- **Minimum API**: Connect IQ 5.0.0
- **Required Permissions**:
  - Background (background processes)
  - Communications (weather data)
  - ComplicationSubscriber (complications)
  - Positioning (GPS/location)
  - SensorHistory (sensor history)
  - UserProfile (user profile)

---

## Main Features

### 1. Time Display

- 12h or 24h format
- Seconds display (3 modes)
- Optional leading zero for hours
- AM/PM support in 12h format
- Independent colors configuration (hours, minutes, seconds, separators)

### 2. Circular Data Fields

Four circular data fields positioned at 9h, 11h, 1h and 3h around the watch face:

- Value display
- Customizable title
- Unit display
- Multiple display modes
- Independent colors

### 3. Classic Data Fields

Six peripheral data fields:

- 3 top fields (left, center, right)
- 3 bottom fields (left, center, right)
- Colored icons
- Text values

### 4. Text Fields

- Top text field
- Bottom text field
- Full content customization
- Various display modes

### 5. Information Indicators

Five visual indicators:

1. **Bluetooth**: Phone connection status
2. **Info 2**: Top left
3. **Info 3**: Top right
4. **Info 4**: Left side of date
5. **Info 5**: Right side of date

### 6. Goal Bar

- Graphical progress visualization
- Multiple goal types
- Configurable text and icon
- Customizable colors (empty/filled/text)

### 7. Date

- 7 display formats
- Day of the week
- International format support
- Customizable color

### 8. Weather

- **Sources**: Garmin Weather and/or OpenWeatherMap
- **Available Data**:
  - Current, feels like, min/max temperature
  - Weather description and icon
  - Humidity
  - Wind speed and direction
  - Atmospheric pressure (OWM)
  - Cloud coverage (OWM)
  - Visibility (OWM)
  - Precipitation probability (GW)

---

## User Interface

### Screen Structure

![Watch Face Layout](docs/images/Display_Overview_2.png)

*FUSION IV display layout showing all configurable zones*

### Display Modes

#### Full Display Mode
![Full Display](docs/images/Display_1.png)

#### Always Active Mode
![Always Active](docs/images/Layout_Always_Active.png)

#### Screen Saver Mode
![Screen Saver](docs/images/Layout_Screen_Saver.png)

#### AOD (Always On Display)
![AOD Mode](docs/images/Display_AOD.png)

### Legend
- **Time**: Time display
- **Date**: Date display
- **Circ**: Circular fields
- **TL/TC/TR**: Top fields (Left/Center/Right)
- **BL/BC/BR**: Bottom fields (Left/Center/Right)
- **I2/I3/I4/I5**: Information indicators
- **Goal Bar**: Goal progress bar

---

## Configuration

### System Settings

#### Data Refresh Rate
Controls data update frequency:

- **Full Refresh**: Complete update every second (maximum consumption)
- **High Refresh Rate**: High refresh
- **Medium Refresh Rate**: Medium refresh (recommended)
- **Low Refresh Rate**: Low refresh (battery saving)

#### Power Saving

**Screen Saver Delay**: Delay in minutes before screen saver activation (-1 to disable)

**Screen Off Delay**: Delay in minutes before screen turns off (-1 to disable)

#### Widget

**Launch Widget On Press Hold**: Launch widget on long press (touchscreen only)

---

### Display Settings

#### Time Format

**Use Military Format**: 
- `true`: 24-hour format
- `false`: 12-hour format (AM/PM)

**Hours Leading 0**: 
- `true`: Display leading zero (01, 02, 03...)
- `false`: No leading zero (1, 2, 3...)

**Seconds Display Mode**:
1. **Hidden**: Seconds hidden
2. **Normal**: Normal seconds display
3. **Always On**: Always displayed (non-AMOLED only)

#### Date Format

7 available display modes:

1. `[DOW dd Month]`: Mon 15 January
2. `[DOW dd/mm]`: Mon 15/01
3. `[dd/mm/yyyy]`: 15/01/2026
4. `[DOW Month dd]`: Mon January 15
5. `[Month dd DOW]`: January 15 Mon
6. `[DOW mm/dd]`: Mon 01/15
7. `[yyyy/mm/dd]`: 2026/01/15

---

### Data Fields

#### Configuration for Each Field

For each data field, you can configure:

1. **Data Type**: Choose from 73+ types (see Data Types section)
2. **Custom Title**: Free text to replace default title
3. **Display Mode**: How to display the data

#### Display Modes

##### Circular Fields (9h, 11h, 1h, 3h)

0. **Value**: Value only
1. **Title + Value**: Title above value
2. **Value + Unit**: Value with unit
3. **Value + Title**: Value with title below
4. **Title + Value + Title**: Title, value, title

##### Text Fields (Top/Bottom)

0. **Value**: Value only
1. **Title + Value**: Title and value
2. **Value + Unit**: Value with unit
3. **Value + Title**: Value with title
4. **Title + Value + Title**: Complete title
5. **Title**: Title only
6. **Goal**: Goal display
7. **Value / Goal**: Value over goal
8. **Percents Of Goal**: Goal percentage
9. **Remaining**: Remaining to reach goal

##### Goal Bar

- **Display Goal Bar Icon**: Show icon
- **Display Goal Bar Text**: Show text
- **Goal Bar Text Display Mode**: Text display mode (same options as text fields)
- **Goal Range**: Custom range (min/max) - empty to use system goal

---

### Color Customization

FUSION IV offers **28 customizable colors**:

> 💡 **See the complete [Color Palette Reference](docs/COLOR_PALETTE.md) with hex values and visual previews**

#### Base Colors

| ID | Element | Description |
|----|---------|-------------|
| 0 | Background Color | Watch face background color |
| 1 | Circular Arcs Color | Circular arcs color |
| 2 | Circular Fields Sep Color | Circular field separators color |

#### Circular Fields Colors

| ID | Element |
|----|---------|
| 3 | Circular Fields Value Color |
| 4 | Circular Fields Title/Unit Color |

#### Time Colors

| ID | Element |
|----|---------|
| 5 | Time Hours Color |
| 6 | Time Sep Color (separator) |
| 7 | Time Minutes Color |
| 8 | Time Seconds & AM/PM Color |

#### Date Colors

| ID | Element |
|----|---------|
| 9 | Date Color |

#### Text Colors

| ID | Element |
|----|---------|
| 10 | Top Text Color |
| 11 | Bottom Text Color |

#### Indicator Colors

| ID | Element |
|----|---------|
| 12 | Info Off Color |
| 13 | Info 1 On Color (Bluetooth) |
| 14 | Info 2 On Color (Top Left) |
| 15 | Info 3 On Color (Top Right) |
| 16 | Info 4 Color (Date Side Left) |
| 17 | Info 5 Color (Date Side Right) |

#### Classic Fields Colors

| ID | Element |
|----|---------|
| 18 | Classic Fields X6 Text Color |
| 19 | Top Left Field Icon Color |
| 20 | Top Center Field Icon Color |
| 21 | Top Right Field Icon Color |
| 22 | Bottom Left Field Icon Color |
| 23 | Bottom Center Field Icon Color |
| 24 | Bottom Right Field Icon Color |

#### Goal Bar Colors

| ID | Element |
|----|---------|
| 25 | Goal Bar Off Color |
| 26 | Goal Bar On Color |
| 27 | Goal Bar Text Color |

### Predefined Color Palette

The watch face offers **67 predefined colors** organized by family:

<table>
<tr><th>Color Name</th><th>Hex Code</th><th>Preview</th></tr>
<tr><td colspan="3"><strong>Basics</strong></td></tr>
<tr><td>Black</td><td><code>0x000000</code></td><td style="background-color:#000000; width:80px; height:25px;"></td></tr>
<tr><td>White</td><td><code>0xffffff</code></td><td style="background-color:#ffffff; border:1px solid #ccc; width:80px; height:25px;"></td></tr>
<tr><td>Gray</td><td><code>0xaaaaaa</code></td><td style="background-color:#aaaaaa; width:80px; height:25px;"></td></tr>
<tr><td>Gray: Stone Cold</td><td><code>0x555555</code></td><td style="background-color:#555555; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Blues</strong></td></tr>
<tr><td>Blue</td><td><code>0x0000ff</code></td><td style="background-color:#0000ff; width:80px; height:25px;"></td></tr>
<tr><td>Blue: Bohemian</td><td><code>0x0000aa</code></td><td style="background-color:#0000aa; width:80px; height:25px;"></td></tr>
<tr><td>Blue: Cerulean</td><td><code>0x55aaff</code></td><td style="background-color:#55aaff; width:80px; height:25px;"></td></tr>
<tr><td>Blue: Hawaii Morning</td><td><code>0x00aaff</code></td><td style="background-color:#00aaff; width:80px; height:25px;"></td></tr>
<tr><td>Blue: Magic Ink</td><td><code>0x0055ff</code></td><td style="background-color:#0055ff; width:80px; height:25px;"></td></tr>
<tr><td>Blue: Soul Stone</td><td><code>0x0055aa</code></td><td style="background-color:#0055aa; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Greens</strong></td></tr>
<tr><td>Green: Billiard</td><td><code>0x00aaaa</code></td><td style="background-color:#00aaaa; width:80px; height:25px;"></td></tr>
<tr><td>Green: Duck Hunt</td><td><code>0x005500</code></td><td style="background-color:#005500; width:80px; height:25px;"></td></tr>
<tr><td>Green: Illicit Green</td><td><code>0x55ffaa</code></td><td style="background-color:#55ffaa; width:80px; height:25px;"></td></tr>
<tr><td>Green: Lime</td><td><code>0x00ff00</code></td><td style="background-color:#00ff00; width:80px; height:25px;"></td></tr>
<tr><td>Green: Yoshi</td><td><code>0x55aa00</code></td><td style="background-color:#55aa00; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Reds</strong></td></tr>
<tr><td>Red</td><td><code>0xff0000</code></td><td style="background-color:#ff0000; width:80px; height:25px;"></td></tr>
<tr><td>Red: Heartbeat</td><td><code>0xaa0000</code></td><td style="background-color:#aa0000; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Purples/Pinks</strong></td></tr>
<tr><td>Purple: Bellflower</td><td><code>0x5555aa</code></td><td style="background-color:#5555aa; width:80px; height:25px;"></td></tr>
<tr><td>Purple: Cloak and Dagger</td><td><code>0x550055</code></td><td style="background-color:#550055; width:80px; height:25px;"></td></tr>
<tr><td>Purple: Magentle</td><td><code>0xaa00aa</code></td><td style="background-color:#aa00aa; width:80px; height:25px;"></td></tr>
<tr><td>Purple: Poison</td><td><code>0xaa00ff</code></td><td style="background-color:#aa00ff; width:80px; height:25px;"></td></tr>
<tr><td>Pink: Fuchsia Fever</td><td><code>0xff55aa</code></td><td style="background-color:#ff55aa; width:80px; height:25px;"></td></tr>
<tr><td>Pink: Magenta</td><td><code>0xff00ff</code></td><td style="background-color:#ff00ff; width:80px; height:25px;"></td></tr>
<tr><td>Pink: Pac-Man Kiss</td><td><code>0xff00aa</code></td><td style="background-color:#ff00aa; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Yellows/Oranges</strong></td></tr>
<tr><td>Yellow</td><td><code>0xffff00</code></td><td style="background-color:#ffff00; width:80px; height:25px;"></td></tr>
<tr><td>Yellow: Honey and Thyme</td><td><code>0xaaaa00</code></td><td style="background-color:#aaaa00; width:80px; height:25px;"></td></tr>
<tr><td>Orange</td><td><code>0xffaa00</code></td><td style="background-color:#ffaa00; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Browns</strong></td></tr>
<tr><td>Brown: Pepperoni</td><td><code>0xaa5500</code></td><td style="background-color:#aa5500; width:80px; height:25px;"></td></tr>
<tr><td>Brown: Spikey Red</td><td><code>0x550000</code></td><td style="background-color:#550000; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Cyan</strong></td></tr>
<tr><td>Cyan</td><td><code>0x00ffff</code></td><td style="background-color:#00ffff; width:80px; height:25px;"></td></tr>
<tr><td colspan="3"><strong>Custom Colors</strong></td></tr>
<tr><td>Custom Color 1</td><td colspan="2">User-defined via hex code</td></tr>
<tr><td>Custom Color 2</td><td colspan="2">User-defined via hex code</td></tr>
<tr><td>Custom Color 3</td><td colspan="2">User-defined via hex code</td></tr>
</table>

### Special Color Options

**Use Battery Adaptative Color**: Automatically adapts color based on battery level

**Use Weather Colored Icons**: Colors weather icons according to conditions

**Custom Colors**: Define up to 3 custom colors via hexadecimal code (format: `0xffffff` or `ffffff`)

---

### Weather

#### Provider Configuration

**Weather Provider**: Weather service selection

1. **Garmin Weather (GW)**: Native Garmin service
2. **OpenWeatherMap (OWM)**: External service requiring API key
3. **Garmin Weather + OpenWeatherMap**: Garmin priority, OWM complement
4. **OpenWeatherMap + Garmin Weather**: OWM priority, Garmin complement

#### OpenWeatherMap

**Weather Key**: OpenWeatherMap API key (32 characters max)

To obtain an API key:
1. Create an account on [openweathermap.org](https://openweathermap.org)
2. Generate a free API key
3. Copy the key into the settings

**Weather Call**: Displays last API call time (read-only)

---

### Units of Measurement

#### Altitude
- Meters (m)
- Feet (ft)

#### Distance
- Kilometers (km)
- Miles (mi)
- International Nautical Miles (nm)

#### Temperature
- Celsius (°C)
- Fahrenheit (°F)
- Kelvin (°K)

**Temperature Offset**: Temperature sensor correction (numeric value)

#### Pressure
- Hectopascal (hPa)
- Millimeters Of Mercury 0°C (mmHg)
- Inch Of Mercury 0°C (inHg)

#### Weight
- Kilograms (kg)
- Pounds (lbs)

#### Wind Speed
- Meters / Seconds (m/s)
- Kilometers / Hours (km/h)
- Miles / Hours (mi/h)
- Knots (kn)
- Beaufort Scale (bf)

#### Wind Direction
- **Degrees Direction**: Degree display (000-360)
- **Cardinal Direction**: Cardinal display (N, NE, E, SE, S, SW, W, NW)

---

### Advanced Settings

#### Custom Texts

**Custom Text 1 Value**: Free text for custom display  
**Custom Text 2 Value**: Second free text

#### Countdown

**Countdown Target Day**: Countdown target date  
**Countdown Target Hour**: Target time (format HH:mm:ss, e.g.: 14:30:00)

#### Time Zones

Configuration of 4 additional time zones:

- **Time Zone 2**: UTC format (e.g.: +02:00 or -05:30)
- **Time Zone 3**: UTC format
- **Time Zone 4**: UTC format
- **Time Zone 5**: UTC format

Format: HH:mm with + or - sign (e.g.: `+02:00`, `-05:30`)

#### Icon Sets

**Icons Set**:
- **Filled Icons**: Solid icons
- **Outlined Icons**: Outlined icons

#### Font Ratios

Adjust font sizes independently (75% to 150%):

- **Date Font Ratio**: Date size (75-130%)
- **Text Font Ratio**: Text size (75-130%)
- **Circular Fields Font Ratio**: Circular fields size (75-130%)
- **Classic Fields Font Ratio**: Classic fields size (75-130%)
- **Goal Bar Font Ratio**: Goal bar text size (75-150%)

---

## Available Data Types

FUSION IV supports **73+ different data types**. Here is the complete list:

### Physical Activity

| Type | Description |
|------|-------------|
| Active Minutes : Daily | Daily active minutes |
| Active Minutes : Weekly | Weekly active minutes |
| Calories : Daily Burned | Daily burned calories |
| Calories : Daily Burned Active | Active burned calories |
| Steps Daily | Daily step count |
| Distance : Daily | Today's distance |
| Distance : Weekly | This week's distance |
| Floors Climbed : Daily | Today's climbed floors |

### Specific Distances

| Type | Description |
|------|-------------|
| Bike Distance : Week | Week's cycling distance |
| Bike Distance : 30 Days | 30-day cycling distance |
| Bike Distance : Current Month | Current month's cycling distance |
| Run Distance : Week | Week's running distance |
| Run Distance : 30 Days | 30-day running distance |
| Run Distance : Current Month | Current month's running distance |
| Pushes | Number of pushes (if available) |
| Pushes Distance Daily | Daily push distance |

### Health and Wellness

| Type | Description |
|------|-------------|
| Heart Rate | Current heart rate |
| Heart Rate Min/Max (4 Hours) | HR min/max over 4 hours |
| Body Battery | Body battery level |
| Stress Level | Stress level |
| Respiration Rate | Respiration rate |
| Oxygen Saturation | Oxygen saturation (SpO2) |
| Recovery Time | Recovery time (hh:mm) |
| Weight | Weight in kg |

### Sports Performance

| Type | Description |
|------|-------------|
| VO2 Max Cycling | Cycling VO2 Max |
| VO2 Max Running | Running VO2 Max |
| Race Predictor 5K | 5K time prediction |
| Race Predictor 10K | 10K time prediction |
| Race Predictor Half Marathon | Half marathon prediction |
| Race Predictor Marathon | Marathon prediction |
| Training Status | Training status |

### System and Battery

| Type | Description |
|------|-------------|
| Battery In Days | Battery life in days |
| Battery In Percents | Battery level in % |
| Solar Intensity | Solar intensity |
| Phone Connected | Phone connected |
| Alarms Count | Number of alarms |
| Notifications Count | Number of notifications |
| Move Alert Level | Move alert level |
| Do Not Disturb Enabled | Do not disturb enabled |

### Environment

| Type | Description |
|------|-------------|
| Altitude | Current altitude |
| Pressure From Sensor | Atmospheric pressure |
| Temperature From Sensor | Sensor temperature |

### Weather (Garmin Weather)

| Type | Description |
|------|-------------|
| Weather Description | Weather description |
| Weather Temperature | Weather temperature |
| Weather Temperature : Feel | Feels like temperature |
| Weather Temperature : Min / Max | Min/max temperatures (GW only) |
| Weather Humidity | Humidity |
| Weather Precipitation Probability | Precipitation probability (GW) |
| Weather Wind Speed/Direction | Wind speed and direction |
| Weather GW Update Time | Garmin Weather update time |

### Weather (OpenWeatherMap)

| Type | Description |
|------|-------------|
| Weather Station | Weather station (OWM) |
| Weather Clouds Cover | Cloud coverage (OWM) |
| Weather Pressure | Pressure (OWM) |
| Weather Visibility | Visibility (OWM) |
| Weather OWM Update Time | OpenWeatherMap update time |

### Sun and Moon

| Type | Description |
|------|-------------|
| Sun Event : Daily Sunrise | Sunrise |
| Sun Event : Daily Sunset | Sunset |
| Sun Event : Next Sun Event | Next sun event |
| Sun Event : Civil Dawn | Civil dawn |
| Sun Event : Civil Dusk | Civil dusk |
| Moon Age | Moon age |
| Moon Illumination | Moon illumination |
| Moon Phase | Moon phase |

### Date and Time

| Type | Description |
|------|-------------|
| Date | Current date |
| Day Of The Year | Day of the year |
| Week Of The Year | Week of the year |
| Time Zone 2 | Time zone 2 |
| Time Zone 3 | Time zone 3 |
| Time Zone 4 | Time zone 4 |
| Time Zone 5 | Time zone 5 |
| Countdown | Countdown |

### Customization

| Type | Description |
|------|-------------|
| Custom Text | Custom text 1 |
| Custom Text 2 | Custom text 2 |
| Hidden Field | Hidden field |

### Debug

| Type | Description |
|------|-------------|
| Debug Data | Debug data |

---

## License and Activation

### License Key

**License Key**: Field to enter your license key (15 characters max)

FUSION IV watch face can work in free mode with some limitations. A license unlocks all premium features.

### Obtaining a License

To obtain a license key:
1. Visit the developer's website
2. Follow purchase/activation instructions
3. Enter the key in the watch face settings

### Version Information

**Release**: Displays current watch face version (read-only)

---

## Installation

### Via Garmin Connect IQ Store

1. Open **Garmin Connect** or **Garmin Connect IQ** app
2. Search for "**FUSION IV**"
3. Tap **Install**
4. Wait for synchronization with your watch
5. Select the watch face from your watch settings

### Via Garmin Express (PC/Mac)

1. Connect your watch to the computer
2. Open **Garmin Express**
3. Access **Connect IQ Store**
4. Search and install **FUSION IV**
5. Synchronize

### Initial Setup

After installation:

1. On your watch: **Long press** the button or screen on the watch face
2. Select **Settings**
3. Or configure via **Garmin Connect** > **Connect IQ** > **FUSION IV** > **Settings**

---

## Support and Assistance

### Common Issues

#### Weather is not displaying

**Solution**:
1. Check that location is enabled
2. Ensure phone is connected
3. For OpenWeatherMap: verify API key
4. Wait a few minutes after installation

#### Watch face consumes too much battery

**Solutions**:
- Reduce refresh rate (Low or Medium)
- Enable Screen Saver Delay
- Hide seconds or use "Normal" mode
- Reduce number of active data fields

#### Data is not updating

**Solutions**:
- Increase refresh rate
- Check watch face permissions
- Restart watch

#### Some data shows "---" or is empty

**Cause**: Data not available on your watch model or sensor not present

**Solution**: Replace with another compatible data type

### Debug

The **Debug Data** data type allows displaying diagnostic information:

**Debug Data Type**:
- Location: GPS coordinates
- Location Age: GPS position age (seconds)
- OWM Call Status: OpenWeatherMap call status
- License Infos: License information

### Contact

For any question, suggestion or problem:

- **GitHub Issues**: [Report bugs or request features](https://github.com/Bastos65/Garmin-Watchfaces-Support/issues)
- **Contact**: [Send a message](https://pay.b65dev.com/portfolio/contact)
- **Garmin Forum**: [Fusion IV Discussion](https://forums.garmin.com)

---

## Software License

Copyright © 2026 Bastos65

All rights reserved.

This software and its documentation are protected by copyright. Any unauthorized reproduction, distribution or modification is prohibited.

---

## Changelog

### Beta Version (Current)

#### New Features
- Support for 38 Garmin watch models
- 73+ available data types
- 28 customizable colors
- Dual weather support (GW + OWM)
- Intelligent power saving mode
- 19 supported languages

#### Improvements
- Battery consumption optimization
- Improved performance on AMOLED screens
- Better custom fields management

#### Fixes
- Various bugs fixed

---

## FAQ

### Q: How do I change colors?

**A:** Open settings via Garmin Connect or from the watch, then navigate to the colors section. Each element can be customized independently.

### Q: Can I use OpenWeatherMap for free?

**A:** Yes, OpenWeatherMap offers a free plan with 1000 API calls per day, more than enough for normal usage.

### Q: How many data fields can I display?

**A:** The watch face supports up to 18 configurable data zones simultaneously.

### Q: Does the watch face work offline?

**A:** Yes, only weather data requires a connection. All other data (sensors, activity, etc.) works offline.

### Q: How can I maximize battery life?

**A:** 
- Use "Low Refresh Rate"
- Enable Screen Saver
- Hide or limit seconds display
- Reduce number of displayed fields

### Q: Is my watch model compatible?

**A:** Check the [Compatibility](#compatibility) section to see the complete list of supported watches.

### Q: How do I get help?

**A:** See the [Support and Assistance](#support-and-assistance) section for different support channels.

---

## Glossary

- **AMOLED**: Active Matrix Organic Light-Emitting Diode display type
- **API**: Application Programming Interface
- **Connect IQ**: Garmin platform for third-party applications
- **GW**: Garmin Weather (Garmin weather service)
- **OWM**: OpenWeatherMap (external weather service)
- **SpO2**: Pulse oxygen saturation
- **VO2 Max**: Maximum oxygen consumption
- **UTC**: Coordinated Universal Time

---

## Appendices

### Parameter Formats

#### Custom Colors
Hexadecimal format: `0xRRGGBB` or `RRGGBB`
- RR = Red (00-FF)
- GG = Green (00-FF)
- BB = Blue (00-FF)

Example: `0xFF0000` = Pure red

#### Time Zones
Format: `±HH:mm`
- + sign for East, - for West
- HH = Hours (00-14)
- mm = Minutes (00 or 30)

Examples:
- `+01:00` = UTC+1 (Paris)
- `-05:00` = UTC-5 (New York)
- `+05:30` = UTC+5:30 (India)

#### Countdown Hour
Format: `HH:mm:ss`
- HH = Hours (00-23)
- mm = Minutes (00-59)
- ss = Seconds (00-59)

Example: `14:30:00` = 2:30 PM

### Moon Phase Codes

Moon phases are numbered from 0 to 7:
- 0: New Moon
- 1: Waxing Crescent
- 2: First Quarter
- 3: Waxing Gibbous
- 4: Full Moon
- 5: Waning Gibbous
- 6: Last Quarter
- 7: Waning Crescent

---

**Last updated**: January 2, 2026  
**Document version**: 1.0  
**Author**: Bastos65

---

*This document is provided "as is" without warranty of any kind. The developer reserves the right to modify features and documentation without notice.*
