<p align="center">
  <img src="assets/banner.svg" alt="Landslide and Flash Flood Dashboard banner" width="100%">
</p>

# 🏔️ Landslide \& Flash Flood Early-Insight Dashboard

An interactive R Shiny dashboard that helps anticipate **landslide** and **flash flood** activity across four Himalayan regions of India (Ladakh, Himachal Pradesh, Uttarakhand and Jammu \& Kashmir), using spatial data on rivers, roads, glaciers and terrain.

[!\[R](https://img.shields.io/badge/R-4.x-276DC3?logo=r\&logoColor=white)](https://www.r-project.org/)
[!\[Shiny](https://img.shields.io/badge/built%20with-Shiny-blue)](https://shiny.posit.co/)
\[!\[Course](https://img.shields.io/badge/course-STAT3037A-orange)]()
[!\[License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

<p align="center">
  <img src="https://img.shields.io/badge/status-in%20development-orange?style=for-the-badge" alt="Status: in development">
</p>

<!-- When the app is deployed, replace the badge above with:
<a href="https://YOUR-APP-LINK.shinyapps.io/dashboard/">
  <img src="https://img.shields.io/badge/%F0%9F%9A%80%20Launch%20the%20live%20dashboard-2ea44f?style=for-the-badge" alt="Launch dashboard">
</a>
And add a demo GIF:
<img src="assets/demo.gif" alt="Dashboard demo" width="800">

\---

## 🔍 Overview

Landslides and flash floods are among the most damaging hazards in mountainous and glacier-fed regions. This dashboard brings together river networks, road infrastructure and glacier data so users can explore where hazard activity is most likely and which communities and routes are exposed.

**What you can do with it**

* Explore hazard-relevant layers on an interactive map
* Compare the four study regions side by side
* See which roads and river systems fall in higher-risk areas
* description

### How it works

```mermaid
flowchart LR
    A\[🛰️ Source data<br/>roads, rivers, glaciers] --> B\[🧹 Cleaning in R<br/>sf and tidyverse]
    B --> C\[🗺️ Spatial layers]
    C --> D\[📊 Shiny dashboard]
    D --> E\[👀 Explore hazard areas]
```

### Features

|🗺️ Interactive map|📈 Region comparison|🛣️ Exposure|
|:-:|:-:|:-:|
|Toggle roads, rivers and glacier layers|Compare the four study regions|See which routes sit in higher-risk zones|

\---

## 🗺️ Study regions

|#|Region|Why it matters|
|-|-|-|
|1|**Ladakh**|High-altitude, glacier-rich Union Territory with steep river valleys and exposure to flash floods|
|2|**Himachal Pradesh**|Mountainous state with frequent monsoon landslides along road corridors|
|3|**Uttarakhand**|Glacier-fed rivers and steep slopes, with a history of major flash floods (e.g. Kedarnath 2013, Chamoli 2021)|
|4|**Jammu \& Kashmir**|Himalayan and Pir Panjal terrain, with river basins and road links vulnerable to slope failure and flooding|

\---

## 🛠️ Project status

This dashboard is **under active development**.

* \[x] Collect road, river and glacier datasets
* \[x] Organise repository and documentation
* \[x] Clean and combine spatial layers for the four regions
* \[ ] Build the interactive map
* \[ ] Add region comparison views
* \[ ] Add hazard indicators
* \[ ] Deploy the app online
* \[ ] Add screenshots and a demo GIF

\---

## 🚀 Getting started

### Prerequisites

* R (>= 4.2)
* RStudio or Positron (optional)

### Installation

```r
# Clone the repo, open the project folder in R, then:
renv::restore()
```

### Run the app

```r
shiny::runApp()
```

\---

## 🗂️ Data

<details>
<summary><b>Click to see the datasets used</b></summary>

All source details are listed in [`docs/`](docs/).

|Dataset|Description|Location|
|-|-|-|
|Road networks|Bharatmala and other road networks in India|`data/roads/`|
|Rivers and streams|River network from India-WRIS|`data/rivers/`|
|Boundaries and glaciers|India shapefile and glacier data|`data/boundaries/`|

</details>

\---

## 📁 Project structure

```
.
├── assets/       # Banner and screenshots
├── data/
│   ├── roads/        # Road network data
│   ├── rivers/       # River and stream data
│   └── boundaries/   # India shapefile and glacier data
├── docs/         # Data sources and metadata
├── R/            # R / Shiny code
└── README.md
```

\---

## ⚠️ Limitations

This is an academic project and **not an official early-warning system**. Do not use it to make safety or evacuation decisions. Always follow guidance from national and local disaster management authorities.

\---

## 👥 Team

STAT3037A project team: Hannah Venter, Oratilwe Tau, Sayeeda Naidoo, Nomzamo Dlomo

\---

## 🤝 Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) to get started.

\---

## 📜 License

Released under the [MIT License](LICENSE). Data remains subject to the terms of its original sources (see `docs/`).

