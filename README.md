# Smart-Solar-Charge-Controller
High-efficiency smart solar charge controller with multi-stage battery charging and load management.
# Smart Solar Charge Controller & Energy Management System

A robust, microcontroller-based solar charge controller engineered for standalone photovoltaic (PV) power systems. Focuses on maximum power extraction, adaptive multi-stage battery charging algorithms, and automated system protections for off-grid applications.

## 📌 Project Overview
* **System Type:** Solar PV Power Conditioning & Battery Management System (BMS)
* **Target Chemistries:** Lead-Acid (Flooded/Gel/AGM) and Lithium-based energy storage
* **Core Focus:** High-efficiency buck/switching conversion, precise battery state-of-charge (SoC) monitoring, and intelligent load shedding.

---

## ⚙️ Key Technical Features & Architecture

* **Multi-Stage Battery Charging:** 
  * Bulk stage (constant current) for rapid energy delivery.
  * Absorption stage (constant voltage) to prevent cell degradation.
  * Float/Maintenance stage to counter self-discharge without overcharging.
* **Synchronous Power Switching:** Low-$R_{DS(on)}$ N-channel MOSFET switching topology driven by high-speed gate drivers to minimize conduction and thermal losses.
* **Safety & Protection Layer:**
  * Reverse current flow prevention (night-time battery drain protection).
  * Panel over-voltage clamp and transient surge suppression.
  * Output short-circuit protection and automated low-voltage disconnect (LVD) for load longevity.
* **Telemetry & Feedback:** Real-time analog sensing of panel voltage/current and battery voltage via precision ADC filtering.

---

## 📁 Repository Structure

* `Hardware/` - Power stage schematics, sensor filtering circuitry, and PCB trace sizing notes.
* `Firmware/` - State-machine routines for multi-stage charging, ADC averaging filters, and load control logic.
* `Media/` - Bench-test verification photos, thermal captures under load, and installed field units.

---

## 🛠️ Tools & Technologies Used
* **EDA / Layout:** Proteus Design Suite
* **Control Architecture:** Microcontroller firmware implementing hardware-level protection loops
* **Lab Equipment:** DC Electronic Load, Solar Simulator / Bench Power Supply, Digital Storage Oscilloscope

---

*Note: Proprietary design calculations, complete manufacturing gerbers, and primary switching firmware are withheld. Full IP packages are available upon formal client engagement.*
