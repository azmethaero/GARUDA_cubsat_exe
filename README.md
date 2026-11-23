# GARUDA_cubsat_exe
G.A.R.U.D.A. v3.0 — All-in-One Portable Executable (v1–v3 Complete)

## G.A.R.U.D.A. — All-in-One Portable Release (`GARUDA-portable.exe`)
**Ground-link Automated Receiver & Unified Data Analyzer** · Created by **Niranjan CS**

`GARUDA-portable.exe` bundles the complete G.A.R.U.D.A. CubeSat Testing Facility and Live Telemetry Ground Station into a single standalone Windows executable—combining all features, calibration wizards, safety interlocks, and UI upgrades from Versions 1 through 3.

---

### Complete Version History Included in This Build

#### Version 1 — Core Ground Station & Export Foundation
* **Launch Portal (`index.html`):** Session setup for CubeSat and lab identification.
* **Testing Lab (`testing-lab.html`):** Initial pre-flight health checks, reaction wheel test, and IMU/altimeter calibration.
* **Live Telemetry (`telemetry.html`):** Real-time LoRa-to-USB Web Serial parsing with 3D attitude visualization, map tracking, and live graphing.
* **Auto-Stamped Exports (`assets/garuda.js`):** Exports to CSV, JSON, Excel, and raw logs automatically stamped with CubeSat name, lab name, and timestamp.

#### Version 2 — Guided Calibration Wizards & Safety Interlocks
* **Role-Based Session Routing:** Dedicated entry flows for **CubeSat Testing Facility** (Team Name, Team ID, Lab Name, CubeSat Name) and **Telemetry** (Team Name, Operator Name).
* **Live Sensor Health Checklist:** Top-bar tabbed Testing Facility showing raw data alongside green status indicators and sub-readings for Battery, Accelerometer, Gyroscope, Temperature, Humidity, and Altimeter.
* **Drone-Style Calibration Wizards:** Step-by-step pop-up guides with visual prompts for Altimeter vertical checks, 6-face IMU orientation, and XY/rotational gyroscope tests.
* **Audio, Visual & Actuator Safety:** Quick-test triggers for Buzzer and LEDs, plus a mandatory Reaction Wheel safety interlock modal requiring explicit **"I Understand" → "OK"** confirmation before spin-up.

#### Version 3 — Visual Rebuild, Guided UX & Portable Packaging
* **High-Res Transparent Logos:** Rebuilt day and night logos at 520 px height with true transparency and larger header/modal placement.
* **Unified Controls & Clean Labels:** Consolidated telemetry header buttons into one consistent bar with clear labels (`Live Telemetry`, `Serial & Wheels`, `Both together`, `3D`, `Map & Charts`, `Alerts & Log`).
* **Mobile & Layout Fixes:** Added compact button rows, a swipeable tab strip, and fixed horizontal overflow on the Lab details card.
* **Guided Operator Flow:** Added a unified **Save data** export dropdown, contextual next-step hints, a 4-step **"Let's get started"** onboarding card, test prerequisites/durations, connection locks until the CubeSat is plugged in, and automatic next-step prompts once all sensors are green.

---

### Running `GARUDA-portable.exe` & Current Status 
* **Unsigned Binary Notice:** Because this portable build is not yet code-signed, Windows Defender SmartScreen may display an *"Unknown publisher"* warning on first launch.
* **Verification Status:** All web views (day, night, mobile), 17 IMU calibration steps, altimeter/sound/LED/wheel tests, and metadata-stamped exports passed under simulated CubeSat testing. Native Windows `.exe` execution and live physical hardware testing are still pending—please report any issues in the **Issues** tab.
