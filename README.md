# Wireless EPG-CP — Smart Palate & Speech Analysis System

A static web app starter for a research software demonstrator for individualized EPG-style palate configuration, simulated tongue–palate contact visualization, and speech session documentation.

## Features
- Dashboard and anonymous participant IDs
- Research session creation and recent sessions
- Digital palate measurement form and STL/PLY filename selection
- Configurable illustrative electrode grid
- Interactive four-state EPG-style contact visualization
- Local event log and CSV export
- Sensor CSV import and explicitly labelled simulated sensor values
- Best-effort Web Bluetooth device selection (custom GATT protocol is not implemented)
- Local audio/video previews and metadata associations
- Print-ready research report (browser Print → Save as PDF)
- Responsive layout for laptop and phone

## Run locally
Open `index.html` in a modern browser. For best results, serve it with a local development server such as VS Code Live Server. Data is stored in this browser's local storage.

## GitHub Pages deployment
1. Open repository Settings → Pages.
2. Under Build and deployment, choose **Deploy from a branch**.
3. Choose branch `main` and folder `/ (root)`, then Save.
4. Wait for deployment and open the URL shown on the Pages settings page.

## Known limitations
- STL/PLY upload currently records the filename only; actual 3D mesh rendering is not implemented.
- BLE selection does not mean sensor data is being received. A real implementation needs the device's documented GATT service and characteristic UUIDs and parsing protocol.
- Contact patterns are manually controlled or simulated, not physiological measurements.
- CSV import is a basic parser; verify column mapping and validate test data before research use.
- Audio and video are previewed locally; files are not uploaded, and their contents are not automatically analyzed.
- No diagnosis, treatment recommendation, automatic tongue tracking, or clinical speech score is generated.

## Safety and privacy
This repository contains a research software prototype, not a medical device and not clinically validated software. Do not store names or identifiable child health information. Do not place homemade sensors, batteries, wires or printed parts into a person's mouth. Intraoral development requires qualified dental and biomedical engineering review, biocompatible materials, retention and aspiration risk assessment, electrical/thermal/moisture safety work, ethical review and clinical validation before research use with children.
