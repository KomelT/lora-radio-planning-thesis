# LoRa Radio Planner

Web-based radio modelling and planning tool for LoRa networks, developed as part of a bachelor’s thesis.

�� **Live demo:** https://rf-planner.komelt.dev/

---

## Overview

This project presents the design, development, and evaluation of a web-based radio modelling tool for planning LoRa networks.  
The application integrates the **SPLAT! (Signal Propagation, Loss, And Terrain)** propagation model with an interactive web interface to enable:

- radio coverage prediction,
- line-of-sight (LOS) analysis,
- optimal transmitter placement,
- visualization of results on real terrain data.

The tool is intended to simplify LoRa network planning in geographically complex environments and to bridge the gap between command-line RF modelling tools and modern, user-friendly web applications.

---

## Features

- �� **Radio coverage simulation** based on the Longley–Rice (ITM) propagation model  
- ��️ **Line-of-sight (LOS) analysis** with Fresnel zone visualization  
- ��️ **Interactive map-based interface** for selecting nodes and areas  
- �� **Optimal node placement**
  - from a predefined set of candidate locations
  - from an automatically detected area (terrain-based candidates)
- �� **Real terrain data support** using SRTM elevation models  
- �� **Validation with real-world field measurements**  
- �� **Open-source and extensible architecture**

---

## Architecture

The application follows a modular, service-oriented architecture:

- **Frontend**
  - Vue.js
  - Tailwind CSS
  - MapLibre GL
- **Backend**
  - Python (FastAPI)
  - Asynchronous task execution
- **Simulation engine**
  - SPLAT! / SPLAT-HD
- **Geospatial services**
  - GeoServer (WMS for coverage visualization)
- **Infrastructure**
  - Redis (task and result storage)
  - Nginx (reverse proxy)
  - Docker (containerized deployment)

---

## Live Application

A publicly available instance of the application is deployed at:

�� **https://rf-planner.komelt.dev/**

This instance demonstrates the core functionality of the system, including coverage prediction and line-of-sight analysis.

---

## Academic Context

This project was developed as part of a bachelor’s thesis in Computer Science at the University of Ljubljana, Faculty of Computer and Information Science.

**Thesis title:**  
*Design, Development, and Testing of a Radio Modelling Tool for LoRa Network Planning*

The thesis focuses on:
- evaluating existing RF planning tools,
- extending an open-source base project,
- integrating terrain-aware radio modelling into a modern web application,
- validating simulation results using real measurement data.

---

## License

The source code of this project is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.

This means you are free to:
- use,
- modify,
- and distribute the software,

provided that any derived work is released under the same license.

See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- **Meshtastic community** – for the original Site Planner project  
- **SPLAT!** – RF propagation and terrain analysis tool  
- Open-source GIS and mapping communities whose tools made this project possible

---

## Author

**Tilen Komel**

If you are interested in extending the project or using it for research or educational purposes, feel free to explore the code or get in touch.
