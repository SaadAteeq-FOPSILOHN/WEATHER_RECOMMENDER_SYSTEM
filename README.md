Weather Data Analysis Project (2023)
Daily Meteorological Records from Montreal and Bainbridge Airports
About This Project
This repository contains daily weather observations recorded throughout 2023 at two major airports:

🍁Montreal-Pierre Elliott Trudeau International Airport (Quebec, Canada)

🌞 Bainbridge Industrial Air Park (Georgia, USA)

I compiled this dataset to analyze regional climate patterns, compare extreme weather events, and practice data cleaning/visualization techniques. The raw data comes from official meteorological sources but has been merged and standardized for easier analysis.

What's in the Data?
Key Features:
✅ Temporal Coverage: Full year of 2023 (365 days per station)
✅ Core Measurements:

Temperature (°F/°C)

Precipitation (inches/mm)

Wind speed & direction

Humidity/dew point

Atmospheric pressure

File Details:
📄 Filename: combined_weather_data.csv
🔢 Records: ~730 (2 stations × 365 days)
📏 Variables: 30+ columns (see full list below)

### Key Features (Measured Variables):
- **Temperature Metrics**:  
  `TEMP` (Avg daily temp), `MAX`/`MIN` (Extremes), `DEWP` (Dew point)  
- **Wind & Pressure**:  
  `WDSP` (Wind speed), `GUST` (Peak gust), `SLP` (Sea-level pressure)  
- **Precipitation/Snow**:  
  `PRCP` (Rainfall), `SNDP` (Snow depth), `FRSHTT` (Weather events flag)  
- **Visibility**:  
  `VISIB` (Miles/km)

  
Working with the Data
Quick Start (Python Example):
python
Copy

import pandas as pd

# Load the dataset
weather_df = pd.read_csv("combined_weather_data.csv")

# Filter for Montreal records
montreal_df = weather_df[weather_df['NAME'].str.contains("MONTREAL")]

# Calculate average temperature
print(f"Montreal's 2023 avg temp: {montreal_df['TEMP'].mean():.1f}°C")


Common Use Cases:
Climate Comparison: Contrast temperature trends between coastal (Bainbridge) and inland (Montreal) locations

Extreme Weather Analysis: Identify days with heaviest precipitation or highest winds

Seasonal Patterns: Visualize snow accumulation trends in Montreal

Why This Matters
As someone passionate about environmental science, I created this repository to:
🔍 Practice real-world data skills with authentic meteorological data
🌎 Understand climate differences between geographic regions
📊 Build reproducible analyses that others can extend

Getting Help
Hit a snag? Have ideas to collaborate?
📧 Email: saadateeq412515@gmail.com

"Whether you're a fellow data enthusiast, student, or researcher - I'd love to hear how you're using this dataset!"

Sharing & Attribution
This data is free to use for academic and personal projects. If you find it helpful:

⭐ Star this repo to support visibility

📖 Cite the original sources:

Canada: Environment and Climate Change Canada

USA: NOAA National Centers for Environmental Information

