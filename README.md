# Edge-AI-DevBoard
A 4-Layer HDI custom PCB designed for an STM32-based Edge AI system featuring Via-in-Pad and strict impedance control.

A highly compact, manufacturing-ready 4-layer High-Density Interconnect (HDI) development board designed from scratch using KiCad. The board is architected around an STM32F4 microcontroller and features an integrated CP2102 USB-to-UART bridge.

*(Yahan apna Altium/KiCad ka 3D X-Ray ya board ka screenshot drag karke daal dena)*

## 🚀 Key Hardware Engineering Features
* **4-Layer Stackup:** Implemented dedicated internal Ground (`GND_Plane`) and Power (`+3V3_Power`) planes to minimize loop inductance and ensure strict EMI/EMC compliance.
* **HDI & Via-in-Pad (VIP):** Utilized advanced Blind Vias and Via-in-Pad routing techniques under the CP2102 to maximize spatial efficiency and thermal dissipation.
* **Power Integrity:** Designed localized Switched-Mode Power Supply (SMPS) power islands to isolate switching noise from sensitive digital logic.
* **DFM & Manufacturing:** Generated comprehensive manufacturing outputs (Gerbers, NC Drill files) compliant with epoxy-capped via constraints.

## 🛠️ Toolchain Used
* **EDA Tool:** KiCad 8.0
* **Architecture:** ARM Cortex-M4 (STM32)
* **Key Components:** STM32F401RCTx, CP2102N, TLV62569 (Regulator)

## 📂 Project Structure
* `*.kicad_sch`: Complete Schematic Design
* `*.kicad_pcb`: 4-Layer PCB Layout
* `Gerbers/`: Production-ready fabrication files
