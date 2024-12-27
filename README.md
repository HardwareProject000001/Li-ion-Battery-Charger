# Li-Ion Battery Chargers Project Repository
<p align = "center">
  <img width="182" alt="Screenshot 2024-11-10 at 12 53 51 AM" src="https://github.com/user-attachments/assets/b8019610-3ce6-489b-9841-1c94ead8886b">
</p>
This repository provides project files for building, designing, and testing various Li-Ion battery chargers. It explores multiple charging modules, protection circuits, and Battery Management Systems (BMS) suited for Li-Ion batteries. The main objective is to design efficient and safe charging circuits for Li-Ion cells, especially for configurations like the 5-cell Li-Ion battery charger.

Li-Ion battery chargers are designed to safely recharge Lithium-Ion cells while monitoring charging currents, voltages, and cell health. This process involves controlling voltage and current flows and integrating BMS (Battery Management Systems) to enhance safety and prolong battery life. Different charging modules and integrated circuits (ICs), such as TP4056, MCP73831, and BQ24072, help implement these requirements.

## Table of Contents

1. [About Li-Ion Battery Chargers](#about-li-ion-battery-chargers)
2. [Charging Stages](#charging-stages)
3. [Battery Management Systems (BMS)](#battery-management-systems-bms)
4. [Li-Ion Charging Modules](#li-ion-charging-modules)
    - TP4056 Module
    - MCP73831 Module
    - BQ24072 Module
5. [Project Structure](#project-structure)
6. [Project Files](#project-files)
7. [Usage](#usage)
8. [Contributing](#contributing)
---

## About Li-Ion Battery Chargers

Li-Ion batteries have become the preferred choice for many portable electronic devices due to their high energy density, lightweight, and longer lifespan. However, they require specific charging conditions to maintain their efficiency and safety. Li-Ion battery chargers control the charging voltage and current in a structured manner to avoid overcharging, overheating, and potential damage to cells.

## Charging Stages

Li-Ion battery charging involves three main stages:

1. **Pre-charge** - For batteries below a minimum voltage, a low current is initially applied to gently bring the cell to a safe voltage range.
2. **Constant Current (CC) Charge** - The battery is charged with a constant current until it reaches a specific voltage, typically 4.2V per cell.
3. **Constant Voltage (CV) Charge** - As the cell reaches its target voltage, the charger gradually reduces the current while maintaining a constant voltage. Charging ends when the current drops to a specified cutoff value.

## Battery Management Systems (BMS)

A Battery Management System (BMS) is essential in multi-cell setups, as it ensures safety and cell longevity by monitoring each cell's voltage, temperature, and charge/discharge rates. Key features include:

- **Overvoltage Protection** - Prevents charging cells beyond their maximum voltage.
- **Undervoltage Protection** - Ensures cells do not discharge below a safe limit.
- **Overcurrent Protection** - Limits high current draw, protecting cells from damage.
- **Balancing** - Equalizes the charge across all cells to maintain consistency in multi-cell configurations.

## Li-Ion Charging Modules

The following modules are popular for implementing safe Li-Ion charging circuits and come with integrated protection features.

- **TP4056** : This module is widely used for single-cell Li-Ion charging with a micro-USB interface. It offers built-in overcharge and over-discharge protection.
  <p align = "center">
    <img width="210" alt="384656458-b03900a7-901a-4d6e-81bf-0546a2f1e60c" src="https://github.com/user-attachments/assets/affbbc74-1575-4684-9ae8-d33e9a75b677" />
  </p>

- **MCP73831** : A compact solution for single-cell charging with reliable current control and thermal regulation.
 <p align = "center">
   <img width="272" alt="384656539-2cd9135c-0f03-4d54-9731-f1ee62bc58b5" src="https://github.com/user-attachments/assets/547f16f9-b269-4159-97bc-0bd1dee9d227" />
 </p>
 
- **BQ24072**: This module is designed for portable applications, offering features like cell balancing and protection for multi-cell setups.
<p></p>
<p align = "center">
  <img width="301" alt="384656639-a15c5106-b2f6-4808-8509-de0aa4af84aa" src="https://github.com/user-attachments/assets/bcb614b0-3ee2-4952-8d48-fa20f3086807" />
</p>
<hr>
## Project Structure

This repository is organized by individual project folders, each covering different aspects of Li-Ion battery charger design.

```plaintext
Li-Ion-Battery-Charger-Projects/
├── 5-Cell-Li-Ion-Battery-Charger/
│   ├── Circuit Diagrams/
│   ├── Datasheets/
│   ├── Pictures/
│   │   ├── Component_Images/
│   │   └── Project_Images/
│   ├── Finance.xlsx
│   └── Report.docx
└── README.md
```


### Folder Descriptions

- **Circuit Diagrams**: Contains schematic designs for the charger circuit, including wiring and component details.
- **Datasheets**: Houses datasheets for components used in each project, providing technical specifications.
- **Pictures**: Organized into:
  - **Component Images**: Photos of components used in the circuit.
  - **Project Images**: Images showing the assembled project and any testing setups.
- **Finance.xlsx**: A spreadsheet documenting the expenses for each project.
- **Report.docx**: A detailed report on the project, including technical analysis, test results, and conclusions.

## Project Files

Each project includes necessary files such as circuit diagrams, datasheets, images, financial records, and reports. Review these files to gain a comprehensive understanding of each charger design and build.

### Project: 5-Cell Li-Ion Battery Charger

This project demonstrates a multi-cell charging system for a 5-cell Li-Ion configuration, covering essential components, BMS integration, and voltage/current regulation. The Circuit Diagrams folder provides schematics for a 5-cell charging circuit with protection features and voltage control.

<p align = "center">
  <img width="1477" alt="384656374-9ee66099-9fa5-496d-8382-110742835494" src="https://github.com/user-attachments/assets/89d278f7-0bd8-47d0-8e46-41c2ed64c7de" />
</p>

## Usage

To use any project in this repository:
1. Download or clone the repository.
2. Navigate to the project folder of interest.
3. Review the **Report.docx** file for a complete understanding of the design and specifications.
4. Follow the **Circuit Diagrams** for wiring and assembly, using datasheets for reference on each component's capabilities.

## Contributing

Contributions are welcome! Feel free to submit pull requests for new charging modules, optimized circuits, or corrections to existing designs. Please ensure any additional files are properly organized within the folder structure.
