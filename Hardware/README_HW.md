# Flipper Zero CAN FD HS 

<div align="center">
  <img src="/Pictures/HW_Banner.png" alt="">
</div>

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Hardware Specifications](#hardware-specifications)
4. [Directory Structure](#directory-structure)
5. [Getting Started](#getting-started)
6. [Hardware Design Files](#hardware-design-files)
7. [Bill of Materials (BOM)](#bill-of-materials)
8. [Software & Firmware](#software--firmware)
9. [Testing & Debugging](#testing--debugging)
10. [Contributing](#contributing)
11. [License](#license)
12. [Contact](#contact)

---

## Project Overview

The Flipper Zero CAN FD/HS Module is an open-source hardware project focused on developing a custom electronic board that serves enables Flipper Zero to communicates with devices with a CAN interface. 

This repository contains the hardware design files, including schematics, PCB layout, and other resources necessary for the development and manufacturing of the board.

## Features
  - Supports both CAN 2.0B and CAN FD (up to 8 Mbps)
  - Compact design
  - Low power consumption
  - On-board 5V - 5V DCDC Regulator
  - Galvanic CAN Bus Isolation
  - TX/RX CAN Activity LED
  - Screwless CAN Connector    
 
## Hardware Specifications
- **CAN Controller:** MCP2518FD
- **CAN Transreceiver:** TJA1051i
- **Communication Interfaces:** SPI
- **Power Consumption:** [Idle, Active, etc.]
- **Dimensions:** 68mm x 18mm

## Board Pinout

<div align="center">
  <img src="/Pictures/Connection_wo_Flipper.png" alt="Pinout"  style="width: 700px;">
</div>

## Directory Structure
```
├── /docs/                 # Documentation, guides, and tutorials
├── /hardware/             # Schematic, PCB layout files, gerber files
│   ├── /schematics/       # Schematics files (.pdf)
│   ├── /KiCAD Project/    # PCB & Schematic layout files (.brd, .sch)
│   ├── /gerbers/          # Gerber files for manufacturing
├── /bom/                  # Bill of Materials (BOM) files
└── README_HW.md           # Project documentation (this file)
```

## Getting Started
To start working on this project, clone the repository:
```bash
git clone https://github.com/yourusername/electronic-board-project.git
```

### Prerequisites
- **ECAD Tool**: [ See Getting started with Kicad v7 tutorial](https://docs.kicad.org/7.0/en/getting_started_in_kicad/getting_started_in_kicad.html) 

### Installation
1. Open the `Flipper_Zero_CAN_Module.kicad_pro` file using Kicad v7.x
2. Edit the schematic using the Schematic Editor
3. Edit the PCB using the Pcb Editor
3. Export gerber files from the PCB design if you wish to manufacture the board.

## Hardware Design Files
- **Schematic:** [Provide details about the schematic, link to key components, etc.]
- **PCB Layout:**   

<div align="center">
  <img src="PCB_Stackup.png" alt="PCB stackup"  style="width: 700px;">
</div>

- **Gerber Files:** These files are located in `/hardware/gerbers/` and are used for manufacturing the board.

## Bill of Materials (BOM)

The Bill of Materials (BOM) is located in the `/bom/` folder. This includes a list of all components used in the design along with part numbers, quantities, and suppliers.
- Bills of materials is available for this distributor list : 
  - [x] Mouser
  - [x] LCSC
  - [ ] Radiospare
  
## Software & Firmware
[See Software development folder for more information](https://example.com/redirect) 

## Testing & Debugging
Work in progress..  

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`.
3. Make your changes and commit them.
4. Push to the branch: `git push origin feature-branch`.
5. Submit a pull request.

For large features or changes, consider creating an issue first to discuss the idea.

## License
This project is licensed under the TODO. See the [LICENSE](LICENSE) file for details.

---

Feel free to modify this template based on the specifics of your project!