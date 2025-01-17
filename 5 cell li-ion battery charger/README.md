# 5-Cell Li-Ion Battery Charger
<p align = "center">
<img width="1473" alt="392144172-2dc11933-ad47-48b5-9a5d-3c796501af68" src="https://github.com/user-attachments/assets/bd4e764e-8371-44b9-aeef-20b2eb5fc74f" />
</p>
This project involves creating a charger for 5 lithium-ion cells (18650 type) that can charge them simultaneously. The charging process uses a Li-Ion charging module (TP4056) and can charge at a current of 1A per cell. This charger is designed to charge cells commonly used in electric vehicles and other applications. 

---

## Table of Contents

- [Introduction](#introduction)
- [Components Required](#components-required)
  - [Components Information](#components-information)
- [Procedure](#procedure)
  - [Circuit Diagram](#circuit-diagram)
- [Test Results](#test-results)
  - [Test 1](#test-1)
  - [Test 2 (Open Box Test)](#test-2-open-box-test)
  - [Test 3 (Close Box Test)](#test-3-close-box-test)
- [Final View](#final-view)
- [Conclusion](#conclusion)

---

## Introduction

This small but efficient project allows for the charging of five 18650 lithium-ion cells simultaneously. The system uses five TP4056 Li-Ion charging modules, powered by a 12V SMPS (Switched Mode Power Supply) providing 5A. This charger is capable of handling a maximum charging current of 1A per cell.

---

## Components Required

1. **12V/5A SMPS** (X1)
2. **Li-ion Charging Module (TP4056)** (X5)
3. **Customized Board** (X1)
4. **Switch** (X1)
5. **2 Pin AC Power Socket** (X1)
6. **2 Pin AC Power Cable** (X1)
7. **Multi-Color Single Strand Wire** (5 meters)
8. **Cell Holders (for 18650 cells)** (X5)
9. **Nuts and Bolts** (X5)
10. **PVC Box** (X1)
11. **7805 Voltage Regulator** (X5)
12. **Capacitor (10uF/16V)** (X5)

---

### Components Information

#### 1. **12V/5A SMPS**
<p align = "center">
<img width="996" alt="392145349-c27f66fe-6ad6-4bca-ad60-23b012f579d0" src="https://github.com/user-attachments/assets/fbe0d2c5-3d89-489b-b68a-a58a8f78cf2e" />
</p>
This is used to supply 60W of power. It provides better protection compared to a traditional charger. It converts the AC input to 12V DC output, suitable for powering the entire system.

#### 2. **Li-ion Charging Module (TP4056)**
<p align = "center">
<img width="340" alt="392145776-45154ede-0316-4c03-b1f4-74bfdcf01d08" src="https://github.com/user-attachments/assets/cb3e3f09-6412-48f1-9d47-d6fc3b58e256" />
</p>
The TP4056 module is a complete constant current-voltage linear charging module for single-cell 3.7V lithium batteries. It protects against overcharging and undercharging and indicates charging status with a red LED (charging) and blue LED (charging complete). Each module can handle up to 1A of charging current.

**Specifications:**
- Input voltage: 4.5V – 5.5V
- Full charge voltage: 4.25V
- Charging indication: Red LED
- Charging complete indication: Blue LED

#### 3. **Customized Board**
<p align = "center">
<img width="1396" alt="392146341-ec24b2fa-1ca2-4065-8e7b-bfb85e3c2aea" src="https://github.com/user-attachments/assets/3c10d55a-8184-4a39-a826-d595f594bbfe" />
</p>
This board is designed to convert the 12V input to 5V and distribute 5A of current to the 5 TP4056 modules. It uses 7805 voltage regulators, each providing 1A of current, and is equipped with a fan to dissipate the heat generated by the voltage regulators.

#### 4. **Switch (6A 250V ON/OFF Rocket Switch)**
<p align = "center">
<img width="340" alt="392146770-dcea33aa-0074-4564-9ae7-0585a010c3f7" src="https://github.com/user-attachments/assets/a9fb6b9f-bf83-4307-bb8b-3802d196d6ec" />
</p>
Used to control the power supply from the SMPS.

#### 5. **2 Pin AC Power Socket and Cable**

<p align = "center">
<img width="287" alt="392148076-dbea9b78-2c43-4935-a0c9-edd82262c772" src="https://github.com/user-attachments/assets/e9941c75-8df1-4693-9d18-d8fa85c4393a" />
<img width="183" alt="392148209-2d052cfa-b578-47cf-9838-3194f6d290ee" src="https://github.com/user-attachments/assets/632e2caa-e81c-451a-8ee7-ddf90dbff7c9" />
</p>

Used to supply the AC power to the SMPS.

#### 6. **18650 Cell Holders**
<p align = "center">
<img width="224" alt="392148945-80b88148-dd53-480e-8e48-368e33a6333c" src="https://github.com/user-attachments/assets/d6d90a96-1ae1-4071-a647-06cf43a0a1b6" />
</p>
Cell holders make it easy to insert or remove the 18650 cells for replacement or maintenance.

#### 7. **PVC Box**
Used to house all components securely.

---

## Procedure

### 1. Prepare the PVC box
- Drill holes for the switch and 2-pin AC power socket.

### 2. Wiring the Power Supply
- Connect the 220V AC input from the AC power cable to the SMPS, ensuring proper wiring for safety.
  
### 3. Connect the Circuit
- Connect the power from the SMPS to the customized board, which will then distribute power to the TP4056 modules.

### 4. Install the Circuit in the PVC Box
- Place the connected circuit into the PVC box and ensure that the heat sink has enough ventilation for heat dissipation.

### 5. Connect the TP4056 Modules
- Use cell holders for connecting the TP4056 charging modules to the 18650 cells. Ensure correct polarity.

### 6. Testing the Circuit
- Power up the system by plugging in the 220V AC and verify that the red LEDs on the TP4056 modules are glowing (indicating charging).
- Check the connections to ensure everything is working properly.

---

## Circuit Diagram
<p align = "center"> 
<img width="720" alt="392149249-7e4e0c60-fca6-485c-9145-64d66b70a69b" src="https://github.com/user-attachments/assets/dfd40499-cdb0-43e8-885b-3e098567cc65" />
</p>
<hr>

## Test Results

### Test 1
- **Charging Voltage (TP4056):** 4.25V ± 0.05V
- **Input Power:** 220V AC
- **Charging Voltage:** 5V DC
- **Charging Current:** 1A per module
- **FAN:** ON
- **Test Duration:** 2hrs
- **HeatSink Temperature:**
  - Min: 33.3°C
  - Max: 68°C

**Cell Readings (Initial → Final):**
| Cell | Initial Voltage | Final Voltage |
|------|-----------------|---------------|
| 1    | 3.61V           | 4.15V         |
| 2    | 3.65V           | 4.12V         |
| 3    | 3.24V           | 4.14V         |
| 4    | 3.36V           | 4.03V         |
| 5    | 3.73V           | 4.10V         |

---

### Test 2 (Open Box Test)
- **FAN:** OFF
- **AC Power:** OFF
- **Temperature:**
  - Outside: 43°C
  - Min: 39°C
  - Max: 75°C

**Cell Readings (Initial → Final):**
| Cell | Initial Voltage | Final Voltage |
|------|-----------------|---------------|
| 1    | 4.07V           | 4.18V         |
| 2    | 4.00V           | 4.15V         |
| 3    | 3.76V           | 4.17V         |
| 4    | 3.78V           | 4.12V         |
| 5    | 4.01V           | 4.10V         |

---

### Test 3 (Close Box Test)
- **FAN:** ON
- **AC Power:** ON
- **Test Duration:** 40 min
- **Temperature:**
  - Outside: 40°C
  - Min: 39°C
  - Max: 70°C

**Cell Readings (Initial → Final):**
| Cell | Initial Voltage | Final Voltage |
|------|-----------------|---------------|
| 1    | 4.01V           | 4.16V         |
| 2    | 4.08V           | 4.12V         |
| 3    | 4.08V           | 4.16V         |
| 4    | 4.03V           | 4.13V         |
| 5    | 4.01V           | 4.15V         |

---

## Final View

The final assembly consists of:
- The 12V/5A SMPS providing power.
- The customized board with 7805 regulators and fan for heat dissipation.
- Five TP4056 modules connected to the Li-ion cells.
- Indicators showing the charging status of each cell.
- All components housed within a PVC box for protection.
<p align = "center">  
<img width="738" alt="392149847-7652e480-d175-4628-9358-dde3a5b4f789" src="https://github.com/user-attachments/assets/0c85ae8e-f213-4431-bd74-527dbe46e9b4" />
</p>
<hr>
<p align = "center">
<img width="1398" alt="392150475-4dffe136-4535-47a5-867d-92d163badc64" src="https://github.com/user-attachments/assets/9317aa9e-1a8b-432e-9151-423deaf363b7" />
</p>
<hr>
-> While Charging
<p align = "center">
<img width="720" alt="392150867-9c08ee7f-dde0-439d-840b-7f6c91bfc0e3" src="https://github.com/user-attachments/assets/023c2dd5-e5ee-4362-9a16-78f772626750" />
</p>
-> After Charging is completed
<p align = "center">
<img width="1399" alt="392151252-16fd92af-15bb-46fe-8dff-896bc2212128" src="https://github.com/user-attachments/assets/b2e792c8-73d3-429d-95a4-7c26c911bcc5" />
</p>
<hr>

## Conclusion

This 5-cell Li-ion battery charger project provides an efficient and safe solution for charging 18650 cells. The use of TP4056 modules ensures each cell is charged correctly, while the 7805 voltage regulators and SMPS provide stable power. The design is modular and compact, ideal for anyone looking to create a multi-cell charger for their projects.
