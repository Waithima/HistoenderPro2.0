
# HistoEnder Pro2.0 🔬

**HistoEnder Pro** is an open-source, low-cost automated slide-staining system. By repurposing the precise multi-axis movements of a standard 3D printer, this project makes automated histology workflows accessible to laboratories and researchers with limited budgets. 

It features custom 3D-printable mounts and a bespoke web-based G-code generator to easily program and execute precise staining protocols.

---

## Key Features

* **Hardware Repurposing:** Replaces the traditional 3D printer hotend with a custom mechanism to handle delicate microscope slides.
* **Web-Based G-Code Generator:** A user-friendly web interface to define custom staining times, dipping sequences, and physical agitation movements.
* **Custom Mounting Ecosystem:** Parametric brackets designed in OpenSCAD that securely attach to standard X-axis carriages.
* **Cost-Effective Automation:** Drastically reduces laboratory overhead compared to commercial automated staining equipment.

## Technology Stack

* **Hardware Control:** G-code, Standard 3D Printer Firmware (Marlin/Klipper)
* **Web Interface:** HTML, CSS, JavaScript
* **CAD Modeling:** OpenSCAD

---

## Installation & Setup

### Hardware Configuration

1. Disconnect power and remove the existing hotend and extruder assembly from your 3D printer's X-axis gantry.
2. Print the custom slide holder brackets found in the `/hardware` directory. *(Recommendation: Use a chemically resistant filament like PETG or ABS).*
3. Securely mount the printed brackets to the carriage.
4. Arrange your staining beakers in a defined grid on the printer bed. 
   > ⚠️**Safety Note:** Ensure the heated bed is permanently disabled in the firmware to prevent accidental heating of chemical reagents.

### Software Initialization

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/Waithima/HistoEnder-Pro2.0.git](https://github.com/Waithima/HistoEnder-Pro2.0.git)


## Usage Guide
### Open the web interface in your browser.

1. Input the specific beaker positions (X/Y coordinates) corresponding to your physical bed layout.

2. Define the desired staining durations and plunging depths (Z-axis) for each reagent.

3. Click Generate to compile your inputs into an executable .gcode file.

4. Transfer the generated .gcode file to your 3D printer (via SD card or USB) and execute the staining routine.

## Repository Structure
### Development Roadmap
1. Initial hardware mounting design.

2. Basic X/Y/Z movement mapping for beaker dipping.

3. Development of the web-based G-code compiler.

4. Implement advanced mechanical agitation (shaking/vibrating) algorithms within the G-code compiler.

5. Integrate a visual drag-and-drop bed-layout mapper into the web UI.

6. Expand the library of pre-configured standard protocols (Gram stain, PAS, etc.).

## Contributing
Contributions, bug reports, and feature requests are highly encouraged! Feel free to check the issues page if you want to contribute to making accessible laboratory equipment.

## Author
Geofrey Waithima

Email: jeffwaithima400@gmail.com

GitHub:
