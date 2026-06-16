cat > README.md <<'EOF'
# SOAR

SOAR is an Android application developed as part of a University of Oslo student project in collaboration with Portal Space UiO. The app helps small-scale rocketry teams evaluate weather conditions, find suitable launch windows, and simulate rocket trajectories.

🏆 **Winner of the MET Award 2025**, awarded by the Norwegian Meteorological Institute.

## Features

- Select, save, and manage launch sites on an interactive map
- Fetch weather forecasts from MET Norway APIs
- View hourly and daily weather summaries
- Evaluate launch windows as Safe, Caution, Unsafe, or No Data
- Configure custom weather thresholds for launch evaluations
- Retrieve upper-atmosphere wind and temperature data from GRIB2 sources
- Simulate rocket trajectories using configurable rocket parameters
- Switch between saved launch sites, weather profiles, and rocket configurations

## Tech Stack

- **Language:** Kotlin
- **UI:** Jetpack Compose
- **Architecture:** MVVM
- **Dependency Injection:** Dagger-Hilt
- **Networking:** Ktor
- **Database:** Room
- **Map:** Mapbox SDK
- **Weather Data:** MET Locationforecast API and MET IsobaricGrib / GRIB2 data
- **Build System:** Gradle Kotlin DSL

## Setup

This public version does not include active API keys or tokens.

To run the app, add your own Mapbox access token in `gradle.properties`:

    MAPBOX_ACCESS_TOKEN=YOUR_MAPBOX_ACCESS_TOKEN_HERE

You should also update the MET API User-Agent/contact information where requests are made.

Then open the project in Android Studio, sync Gradle, and run the app on an emulator or Android device.

## Contributors

- Insaaf Mahamud
- Neha Zahid
- Malaika Azam
- Lars Wien Tynes
- Jakob Loe
- Torbjørn Hamre

## Acknowledgments

- **MET Norway / Norwegian Meteorological Institute** for providing weather data and awarding SOAR the **MET Award 2025**
- **Portal Space UiO** for the project case and domain insight
- **Mapbox** for map functionality
- **University of Oslo** for the project framework
