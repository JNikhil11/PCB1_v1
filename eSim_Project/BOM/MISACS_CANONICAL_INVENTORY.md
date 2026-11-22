# MISACS — Canonical Component Inventory & Hardware Manifest

**Project:** Modular Industrial Sensor Acquisition and Control System (MISACS)  
**Program:** FOSSEE eSim Winter Internship 2026 — Screening Task 7: PCB Design using eSim  
**Author / Lead Engineer:** Nikhil J  
**Hardware Baseline:** FROZEN & BIT-IDENTICAL  
**Total Electrical Components:** Exactly 70  
**Total Mechanical Mounting Holes:** 4 (M3, 3.2 mm)  
**Total Hardware Physical Elements:** 74  

---

## 1. Machine-Readable Inventory Table

| Ref | Schematic Value | Assigned Footprint | Manufacturer | MPN | Subsystem | Electrical Function | PCB Present |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :---: |
| **C1** | `100uF_50V` | `Capacitor_SMD:CP_Elec_8x10.5` | Panasonic | `EEE-FK1H101P` | Subsystem 1: 24V Power Input & Protection | Primary 24V Bus Bulk Electrolytic Filter Capacitor (Low-ESR, 50V) | PASS |
| **C2** | `10uF_50V` | `Capacitor_SMD:C_1206_3216Metric` | KEMET | `C1206C106K5RAC7800` | Subsystem 1: 24V Power Input & Protection | Primary 24V Bus High-Frequency Ceramic Bypass Capacitor (X7R 1206) | PASS |
| **C3** | `10uF_16V` | `Capacitor_SMD:C_0805_2012Metric` | Murata | `GRM21BR71C106KE15L` | Subsystem 2: LM2576-5.0 Buck DC-DC Converter | +5V Output High-Frequency Ceramic Bypass Capacitor (X7R 0805) | PASS |
| **C4** | `10uF_16V` | `Capacitor_SMD:C_0805_2012Metric` | Murata | `GRM21BR71C106KE15L` | Subsystem 3: AMS1117-3.3 Linear Regulator | +3.3V LDO Input Decoupling Ceramic Capacitor (X7R 0805) | PASS |
| **C5** | `100nF_50V` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 4: 4–20 mA Current-Loop Receiver | 4-20 mA Input RC Low-Pass Filter Capacitor 100nF 50V X7R 0805 | PASS |
| **C6** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 5: 0–10 V Analog Input Conditioning | 0-10 V Input RC Filter Capacitor 100nF 50V X7R 0805 | PASS |
| **C7** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 6: LMV358 Dual Precision Op-Amp Buffer | LMV358 Op-Amp Power Supply Decoupling Capacitor 100nF 50V X7R 0805 | PASS |
| **C8** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 7: ADS1115 16-Bit Delta-Sigma ADC | ADS1115 ADC Power Supply Decoupling Capacitor 100nF 50V X7R 0805 | PASS |
| **C9** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | ESP32 Power Supply Decoupling Capacitor 100nF 50V X7R 0805 | PASS |
| **C10** | `10uF` | `Capacitor_SMD:C_1206_3216Metric` | KEMET | `C1206C106K4RACTU` | Subsystem 3: AMS1117-3.3 Linear Regulator | +3.3V LDO Output Bulk Ceramic Decoupling Capacitor (16V X7R 1206) | PASS |
| **C11** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | ESP32 VDD33 Decoupling Capacitor 100nF 50V X7R 0805 | PASS |
| **C12** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU EN Reset RC Delay Timing Capacitor 100nF 50V X7R 0805 | PASS |
| **C13** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | ESP32 Decoupling Capacitor 100nF 50V X7R 0805 | PASS |
| **C14** | `220uF_16V` | `Capacitor_SMD:CP_Elec_8x10.5` | Panasonic | `EEE-FK1C221P` | Subsystem 2: LM2576-5.0 Buck DC-DC Converter | +5V Output Bulk Filter Electrolytic Capacitor (Low-ESR, 16V) | PASS |
| **C15** | `100nF` | `Capacitor_SMD:C_0805_2012Metric` | KEMET | `C0805C104K5RACTU` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | ESP32 Decoupling Capacitor 100nF 50V X7R 0805 | PASS |
| **D1** | `SMBJ30A` | `Diode_SMD:D_SMB` | Littelfuse | `SMBJ30A` | Subsystem 1: 24V Power Input & Protection | Power Entry Unidirectional Transient Voltage Suppressor (30V 600W SMB, Clamps @ 48.4V) | PASS |
| **D2** | `SS36` | `Diode_SMD:D_SMC` | Vishay | `SS36-E3/57T` | Subsystem 1: 24V Power Input & Protection | Logic Rail Reverse-Polarity Blocking Diode (60V 3A SMC, +24V_LOGIC_FUSED to +24V_LOGIC_PROT) | PASS |
| **D3** | `GREEN` | `LED_SMD:LED_0805_2012Metric` | Lite-On | `LTST-C170KGKT` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | +3.3V System Power Indicator LED Green 0805 | PASS |
| **D4** | `SMAJ3.3A` | `Diode_SMD:D_SMA` | Littelfuse | `SMAJ3.3A` | Subsystem 4: 4–20 mA Current-Loop Receiver | 4-20 mA Shunt Voltage TVS Clamp Diode 3.3V 400W SMA | PASS |
| **D5** | `BAT54S` | `Package_TO_SOT_SMD:SOT-23` | Diodes Inc. | `BAT54S-7-F` | Subsystem 5: 0–10 V Analog Input Conditioning | 0-10 V Divided Analog Dual Schottky Rail Clamp Diode (SOT-23, to +3V3 and GND) | PASS |
| **D6** | `BLUE` | `LED_SMD:LED_0805_2012Metric` | Lite-On | `LTST-C170TBKT` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU Diagnostic / Telemetry Status Indicator LED Blue 0805 | PASS |
| **D7** | `SM712` | `Package_TO_SOT_SMD:SOT-23` | Littelfuse | `SM712-02HTG` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | Asymmetrical Bidirectional TVS Diode Array for RS-485 Bus (+12V/-7V SOT-23) | PASS |
| **D8** | `SS56` | `Diode_SMD:D_SMC` | Vishay | `SS56-E3/57T` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 Inductive Flyback Clamping Diode 60V 5A SMC (Drain to +24V_ACT1) | PASS |
| **D9** | `YELLOW` | `LED_SMD:LED_0805_2012Metric` | Lite-On | `LTST-C170KSKT` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 Active State Indicator LED Yellow 0805 | PASS |
| **D10** | `SS56` | `Diode_SMD:D_SMC` | Vishay | `SS56-E3/57T` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 Inductive Flyback Clamping Diode 60V 5A SMC (Drain to +24V_ACT2) | PASS |
| **D11** | `YELLOW` | `LED_SMD:LED_0805_2012Metric` | Lite-On | `LTST-C170KSKT` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 Active State Indicator LED Yellow 0805 | PASS |
| **D12** | `SS56` | `Diode_SMD:D_SMC` | Vishay | `SS56-E3/57T` | Subsystem 2: LM2576-5.0 Buck DC-DC Converter | Buck Switching Fast Freewheeling Catch Diode (60V 5A SMC, SW_NODE to GND) | PASS |
| **D14** | `SS56` | `Diode_SMD:D_SMC` | Vishay | `SS56-E3/57T` | Subsystem 1: 24V Power Input & Protection | Power Entry Reverse-Polarity Shunt Diode (60V 5A SMC, Net +24V to GND) | PASS |
| **F1** | `1.1A_PTC` | `Fuse:Fuse_1812_4532Metric` | Bourns | `MF-MSMF110/33X-2` | Subsystem 1: 24V Power Input & Protection | Resettable PTC Fuse 1.1A Hold / 2.2A Trip (Logic Rail Protection, +24V to +24V_LOGIC_FUSED) | PASS |
| **F2** | `5A_FAST_FUSE` | `Fuse:Fuse_2410_6125Metric` | Littelfuse | `0451005.MRL` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Channel 1 Fast-Acting Surface Mount Fuse 5.0A 125V (2410) | PASS |
| **F3** | `5A_FAST_FUSE` | `Fuse:Fuse_2410_6125Metric` | Littelfuse | `0451005.MRL` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Channel 2 Fast-Acting Surface Mount Fuse 5.0A 125V (2410) | PASS |
| **JP1** | `TERM_ENABLE` | `Connector_PinHeader_2.54mm:PinHeader_1x02_P2.54mm_Vertical` | Wurth Elektronik | `61300211121` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | RS-485 Bus 120 Ohm Termination Resistor Enable 2-Pin 2.54mm Header | PASS |
| **J1** | `PWR_IN_24V` | `TerminalBlock_Phoenix:TerminalBlock_Phoenix_MKDS-1,5-2-5.08_1x02_P5.08mm_Horizontal` | Phoenix Contact | `1715721` | Subsystem 1: 24V Power Input & Protection | 24V DC Main Power Entry Screw Terminal (Pins: 1=+24V, 2=GND) | PASS |
| **J2** | `4-20mA_IN` | `TerminalBlock_Phoenix:TerminalBlock_Phoenix_MKDS-1,5-2-5.08_1x02_P5.08mm_Horizontal` | Phoenix Contact | `1715721` | Subsystem 4: 4–20 mA Current-Loop Receiver | 4-20 mA Process Current Loop Input Terminal (Pins: 1=LOOP+, 2=LOOP-) | PASS |
| **J3** | `0-10V_IN` | `TerminalBlock_Phoenix:TerminalBlock_Phoenix_MKDS-1,5-2-5.08_1x02_P5.08mm_Horizontal` | Phoenix Contact | `1715721` | Subsystem 5: 0–10 V Analog Input Conditioning | 0-10 V Process Control Voltage Input Terminal (Pins: 1=VIN, 2=GND) | PASS |
| **J4** | `RS485_BUS` | `TerminalBlock_Phoenix:TerminalBlock_Phoenix_MKDS-1,5-3-5.08_1x03_P5.08mm_Horizontal` | Phoenix Contact | `1715734` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | RS-485 Differential Bus Terminal 3-Pin 5.08mm (Pins: 1=A, 2=B, 3=GND) | PASS |
| **J5** | `OUT1_LOAD` | `TerminalBlock_Phoenix:TerminalBlock_Phoenix_MKDS-1,5-2-5.08_1x02_P5.08mm_Horizontal` | Phoenix Contact | `1715721` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 Load Connection Terminal (Pins: 1=+24V_ACT1, 2=MOSFET1_DRAIN) | PASS |
| **J6** | `OUT2_LOAD` | `TerminalBlock_Phoenix:TerminalBlock_Phoenix_MKDS-1,5-2-5.08_1x02_P5.08mm_Horizontal` | Phoenix Contact | `1715721` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 Load Connection Terminal (Pins: 1=+24V_ACT2, 2=MOSFET2_DRAIN) | PASS |
| **L1** | `100uH_1.7A` | `Inductor_SMD:L_Bourns_SRR1260` | Bourns | `SRR1260-101M` | Subsystem 2: LM2576-5.0 Buck DC-DC Converter | Buck Converter Shielded Power Inductor 100uH 1.7A (SRR1260 SMD) | PASS |
| **Q1** | `IPD50N06S4L-08` | `Package_TO_SOT_SMD:TO-252-2` | Infineon Technologies | `IPD50N06S4L-08` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 N-Channel Power MOSFET 60V 50A 8.4mOhm (TO-252 / DPAK) | PASS |
| **Q2** | `IPD50N06S4L-08` | `Package_TO_SOT_SMD:TO-252-2` | Infineon Technologies | `IPD50N06S4L-08` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 N-Channel Power MOSFET 60V 50A 8.4mOhm (TO-252 / DPAK) | PASS |
| **R1** | `1k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-071KL` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | +3.3V Power LED Current Limiting Resistor 1k 1% 0805 | PASS |
| **R2** | `100R_0.1%` | `Resistor_SMD:R_1206_3216Metric` | Susumu | `RR1220P-101-D` | Subsystem 4: 4–20 mA Current-Loop Receiver | 4-20 mA Precision Current Sense Shunt Resistor 100 Ohm 0.1% 25ppm (0.4V to 2.0V) | PASS |
| **R3** | `1k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-071KL` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | Auxiliary Digital Pull-Up / Current Limiter Resistor 1k 1% 0805 | PASS |
| **R4** | `30k_0.1%` | `Resistor_SMD:R_0805_2012Metric` | Panasonic | `ERA-6AEB303V` | Subsystem 5: 0–10 V Analog Input Conditioning | 0-10 V Input Precision Voltage Divider Upper Resistor 30k 0.1% 25ppm 0805 | PASS |
| **R5** | `10k_0.1%` | `Resistor_SMD:R_0805_2012Metric` | Panasonic | `ERA-6AEB103V` | Subsystem 5: 0–10 V Analog Input Conditioning | 0-10 V Input Precision Voltage Divider Lower Resistor 10k 0.1% 25ppm (4:1 scaling to 0-2.5V) | PASS |
| **R6** | `4.7k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-074K7L` | Subsystem 7: ADS1115 16-Bit Delta-Sigma ADC | I2C Bus SCL Pull-Up Resistor 4.7k 1% 0805 (to +3V3) | PASS |
| **R7** | `4.7k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-074K7L` | Subsystem 7: ADS1115 16-Bit Delta-Sigma ADC | I2C Bus SDA Pull-Up Resistor 4.7k 1% 0805 (to +3V3) | PASS |
| **R8** | `10k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-0710KL` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU EN (Reset) Pull-Up Resistor 10k 1% 0805 (to +3V3) | PASS |
| **R9** | `10k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-0710KL` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU GPIO0 (Boot) Pull-Up Resistor 10k 1% 0805 (to +3V3) | PASS |
| **R10** | `1k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-071KL` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU Status LED Current Limiting Resistor 1k 1% 0805 | PASS |
| **R11** | `120R_1%` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-07120RL` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | RS-485 Bus Differential Termination Resistor 120 Ohm 1% 0805 | PASS |
| **R12** | `390R_0.1%` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-07390RL` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | RS-485 Bus Line A Fail-Safe Pull-Up Resistor 390 Ohm 0.1% 0805 (to +3V3) | PASS |
| **R13** | `390R_0.1%` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-07390RL` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | RS-485 Bus Line B Fail-Safe Pull-Down Resistor 390 Ohm 0.1% 0805 (to GND) | PASS |
| **R14** | `10R` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-0710RL` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 Gate Drive Damping Resistor 10 Ohm 1% 0805 | PASS |
| **R15** | `10k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-0710KL` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 Gate-to-Source Pull-Down Resistor 10k 1% 0805 | PASS |
| **R16** | `2.2k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-072K2L` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch1 LED Ballast Resistor 2.2k 1% 0805 (limits current from +24V rail) | PASS |
| **R17** | `10R` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-0710RL` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 Gate Drive Damping Resistor 10 Ohm 1% 0805 | PASS |
| **R18** | `10k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-0710KL` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 Gate-to-Source Pull-Down Resistor 10k 1% 0805 | PASS |
| **R19** | `2.2k` | `Resistor_SMD:R_0805_2012Metric` | Yageo | `RC0805FR-072K2L` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Actuator Ch2 LED Ballast Resistor 2.2k 1% 0805 (limits current from +24V rail) | PASS |
| **SW1** | `RESET` | `Button_Switch_SMD:SW_SPST_PTS645` | C&K Components | `PTS645SM43SMTR92LFS` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU Hardware Reset Tactile Pushbutton Switch (Active-Low EN) | PASS |
| **SW2** | `BOOT` | `Button_Switch_SMD:SW_SPST_PTS645` | C&K Components | `PTS645SM43SMTR92LFS` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | MCU Boot Mode Select / Download Tactile Pushbutton Switch (GPIO0) | PASS |
| **U1** | `LM2576HVS-5.0` | `Package_TO_SOT_SMD:TO-263-5_TabPin3` | Texas Instruments | `LM2576HVS-5.0/NOPB` | Subsystem 2: LM2576-5.0 Buck DC-DC Converter | Step-Down Switching Voltage Regulator 24V to 5V 3A (TO-263-5, 52 kHz) | PASS |
| **U2** | `AMS1117-3.3` | `Package_TO_SOT_SMD:SOT-223-3_TabPin2` | Advanced Monolithic Systems | `AMS1117-3.3` | Subsystem 3: AMS1117-3.3 Linear Regulator | Low-Dropout Linear Regulator 5V to 3.3V 1A (SOT-223-3, +3V3 Rail) | PASS |
| **U3** | `LMV358` | `Package_SO:SOIC-8_3.9x4.9mm_P1.27mm` | Texas Instruments | `LMV358IDR` | Subsystem 6: LMV358 Dual Precision Op-Amp Buffer | Dual General Purpose Rail-to-Rail Output Op-Amp (SOIC-8, Ch A: 4-20mA, Ch B: 0-10V) | PASS |
| **U4** | `ADS1115` | `Package_SO:MSOP-10_3x3mm_P0.5mm` | Texas Instruments | `ADS1115IDGSR` | Subsystem 7: ADS1115 16-Bit Delta-Sigma ADC | 16-Bit Precision Delta-Sigma ADC with PGA and I2C Interface (MSOP-10, A0=4-20mA, A1=0-10V) | PASS |
| **U5** | `ESP32-WROOM-32` | `RF_Module:ESP32-WROOM-32` | Espressif Systems | `ESP32-WROOM-32E-N16` | Subsystem 8: ESP32-WROOM-32 Microcontroller Core | Dual-Core 240MHz 32-Bit Wi-Fi & BLE Microcontroller Module (16MB Flash, On-Board PCB Antenna) | PASS |
| **U6** | `MAX3485EESA` | `Package_SO:SOIC-8_3.9x4.9mm_P1.27mm` | Analog Devices / Maxim | `MAX3485EESA+` | Subsystem 10: Non-Isolated RS-485 Serial Fieldbus | 3.3V Half-Duplex RS-485/RS-422 Transceiver (SOIC-8, Non-Isolated, SM712 Protected) | PASS |
| **U7** | `UCC27524D` | `Package_SO:SOIC-8_3.9x4.9mm_P1.27mm` | Texas Instruments | `UCC27524D` | Subsystem 9: Dual High-Current MOSFET Actuator Drivers | Dual 5A High-Speed Low-Side Gate Driver (SOIC-8, Driven by MCU PWM) | PASS |
| **U8** | `TPS26610DDF` | `Package_TO_SOT_SMD:SOT-23-8` | Texas Instruments | `TPS26610DDFR` | Subsystem 4: 4–20 mA Current-Loop Receiver | Active 24V Current-Loop Protector & eFuse (SOT-23-8, 30mA Limit & Reverse Blocking) | PASS |
| **H1** | `MountingHole_3.2mm_M3` | `MountingHole:MountingHole_3.2mm_M3` | Mechanical | `M3_PLATED_HOLE` | Mechanical & PCB Fabrication | 3.2 mm Plated M3 Chassis Mounting Hole with corner setback | PASS |
| **H2** | `MountingHole_3.2mm_M3` | `MountingHole:MountingHole_3.2mm_M3` | Mechanical | `M3_PLATED_HOLE` | Mechanical & PCB Fabrication | 3.2 mm Plated M3 Chassis Mounting Hole with corner setback | PASS |
| **H3** | `MountingHole_3.2mm_M3` | `MountingHole:MountingHole_3.2mm_M3` | Mechanical | `M3_PLATED_HOLE` | Mechanical & PCB Fabrication | 3.2 mm Plated M3 Chassis Mounting Hole with corner setback | PASS |
| **H4** | `MountingHole_3.2mm_M3` | `MountingHole:MountingHole_3.2mm_M3` | Mechanical | `M3_PLATED_HOLE` | Mechanical & PCB Fabrication | 3.2 mm Plated M3 Chassis Mounting Hole with corner setback | PASS |

---

## 2. Summary by Component Family

- **Integrated Circuits (8):** U1 (LM2576HVS-5.0), U2 (AMS1117-3.3), U3 (LMV358), U4 (ADS1115), U5 (ESP32-WROOM-32), U6 (MAX3485EESA), U7 (UCC27524D), U8 (TPS26610DDF).
- **Power MOSFETs (2):** Q1, Q2 (IPD50N06S4L-08 60V 50A 8.4mΩ N-Channel in TO-252 / DPAK).
- **Diodes & Protection (13):** D1 (SMBJ30A 30V TVS), D2 (SS36 60V 3A Schottky), D3 (Green LED), D4 (SMAJ3.3A 3.3V TVS), D5 (BAT54S Dual Schottky), D6 (Blue LED), D7 (SM712 RS-485 TVS Array), D8, D10, D12, D14 (SS56 60V 5A Schottky Diodes), D9, D11 (Yellow LEDs).
- **Fuses (3):** F1 (MF-MSMF110/33X-2 1.1A PTC), F2, F3 (0451005.MRL 5.0A Fast Fuse).
- **Passives (35):** 19 Resistors (R1-R19), 15 Capacitors (C1-C15), 1 Inductor (L1 100µH 1.7A).
- **Interconnect & Switches (9):** Connectors J1, J2, J3, J5, J6 (2-pin screw terminals), J4 (3-pin screw terminal), JP1 (2-pin 2.54mm jumper), SW1 (Reset switch), SW2 (Boot switch).
- **Mechanical Mounting (4):** H1-H4 (3.2 mm plated M3 mounting holes).

---

## 3. Critical Verification & Identity Disclosures

1. **Gate Drive & Isolation:** The dual actuator channels are driven by **U7 (UCC27524D)** dual 5A high-speed low-side gate driver. There are **NO optocouplers (PC817)** in the circuit. Gate drive is non-isolated.
2. **Power Switches:** Power switches are **Q1, Q2 (IPD50N06S4L-08)** in TO-252 (DPAK). They are NOT AOD4184A or PSMN022-30PL.
3. **Operational Amplifier:** Analog front-end buffering uses **U3 (LMV358)** dual rail-to-rail op-amp in SOIC-8. It is NOT TLV272.
4. **ADC & MCU Identifiers:** The ADC is **U4 (ADS1115)** in MSOP-10. The on-board microcontroller is **U5 (ESP32-WROOM-32)**. J6 is an actuator output load connector, NOT an MCU header.
5. **Current-Loop eFuse:** The 4–20 mA active protector is **U8 (TPS26610DDF)** in SOT-23-8.
6. **RS-485 Transceiver & Isolation:** RS-485 communication uses **U6 (MAX3485EESA)**. It is **NON-ISOLATED** (shares board ground). It is protected by D7 (SM712 TVS array) and features 120Ω bus termination via JP1 (TERM_ENABLE). It is NOT MAX13487 and is NOT galvanically isolated.
7. **Reviewer Attribution:** External contributors Eyantra698Sumanto and OfficialVarad were independent screening reviewers/auditors on GitHub, NOT project mentors. Author is Nikhil J (Lead Engineer).
