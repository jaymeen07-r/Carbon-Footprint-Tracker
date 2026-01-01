# Carbon Footprint Tracker

The **Carbon Footprint Tracker** is an IoT-powered system designed to measure, analyze, and visualize carbon emissions in real time. It helps users understand their environmental impact and encourages data-driven decisions to reduce their carbon footprint.

---

## Overview

This project combines embedded hardware, on-device machine learning, and a server interface to monitor carbon-related parameters. Sensors capture environmental and usage data, which is processed by a trained model and then sent to a backend for logging, visualization, and insights.

Key capabilities include:
- Real-time carbon emission monitoring using hardware sensors and firmware logic.
- Lightweight ML inference with a pre-trained model deployed on a microcontroller.
- Server-side handling of data for storage, visualization, and further analysis.

---

## Features

- **IoT-based data collection**: Hardware setup captures relevant environmental and usage metrics via sensors and microcontroller firmware.
- **On-device ML model**: `model.h` contains the exported model for inference on the device, enabling low-latency predictions and reduced network dependency.
- **Firmware integration**: `server.ino` and `firmware.bin` orchestrate sensor reading, prediction, and data transmission to the server.
- **Visualization-ready data**: The system is structured so that collected data can be plugged into dashboards or analytics tools to extract insights on carbon footprint trends.
- **Modular structure**: Training assets, firmware, and server code are separated for easier iteration and maintenance.

---

## Project Structure

- `Model Training.zip`  
  Contains training scripts, datasets, and notebooks for building and evaluating the carbon footprint prediction model.

- `model.h`  
  Exported C/C++ header file of the trained model for deployment on the microcontroller.

- `firmware.bin`  
  Compiled firmware binary that can be flashed onto the device to run the tracker.

- `server.ino`  
  Arduino/ESP sketch responsible for:
  - Reading sensor data.  
  - Running inference using `model.h`.  
  - Communicating with the backend or client interface.

- `circuit_image.png`  
  Circuit diagram or reference image illustrating the hardware connections and sensor layout.

- `README.md`  
  Documentation and high-level description of the project, architecture, and usage.

---

## Use Cases

- **Personal sustainability tracking**: Individuals can track their own device or household-level impact and adjust habits accordingly.
- **Educational projects**: Demonstrates end-to-end IoT + ML workflow, from model training to deployment on a microcontroller.
- **Prototype for smart infrastructure**: Can serve as a starting point for integrating carbon tracking into smart homes, offices, or campuses.
- **Research and experimentation**: Offers a base for experimenting with different models, sensors, or data sources related to emissions.

---

## Demo

A video demonstration of the project is available here:  
[Project Video (Google Drive)](https://drive.google.com/file/d/1ZT_seSBor3EbBIRtaZ-bxRdfjx3cjlOa/view?usp=sharing)

---

## Team

- **Team Name**: Greensync  
- **Team Number**: 24  
