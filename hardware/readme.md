**Hardware Design** 

pixhawk 5x standard :
- specs  [[Pixhawk DS-011]](https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-011%20Pixhawk%20Autopilot%20v5X%20Standard.pdf)
- Bus  [[Pixhawk DS-010]](https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-010%20Pixhawk%20Autopilot%20Bus%20Standard.pdf)
- connector [[Pixhawk DS-009]](https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-009%20Pixhawk%20Connector%20Standard.pdf)

**Component**

Processor 
- STM32F765x - flight-processor [[datasheet]](https://www.st.com/resource/en/datasheet/stm32f765ii.pdf) - [details](https://github.com/rizki-ap/Flight-Controller/blob/main/hardware/FlightMCU.md)
- STM32f103x - IO-processor [[datasheet]](https://www.st.com/resource/en/datasheet/stm32f103c8.pdf) - [details](https://github.com/rizki-ap/Flight-Controller/blob/main/hardware/IoMCU.md)

Sensors :
- ICM‑20689 - 3‑axis gyro + 3‑axis accel, SPI-if [[datasheet]](https://product.tdk.com/system/files/dam/doc/product/sensor/mortion-inertial/imu/data_sheet/ds-000143-icm-20689-datasheet.pdf)
- ICM‑42688‑P - 6-Axis MEMS MotionTracking [[datasheet]](https://product.tdk.com/system/files/dam/doc/product/sensor/mortion-inertial/imu/data_sheet/ds-000347-icm-42688-p-v1.6.pdf)
- BMI088 - 6-axis motion tracking [[datasheet]](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bmi088-ds001.pdf)
- MS5611‑01BA03	- Barometric pressure sensor (I²C/SPI)	[[Datasheet]](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=showdoc&DocId=Data+Sheet%7FMS5611-01BA03%7FB3%7Fpdf%7FEnglish%7FENG_DS_MS5611-01BA03_B3.pdf)
- IST8310	- 3‑axis magnetometer (I²C)	[[Datasheet]](https://www.isentek.com/api/download?url=https%3A%2F%2Fassets.isentek.com%2Fpublic%2Fdocuments%2Fdatasheet%2FHFH0n8I7hQ-IST8310_Datasheet_V1.8_Web.pdf&filename=IST8310_Datasheet_V1.8_Web.pdf&action=view)

Memory :
- W25Q128JVSIM (or JVSIQ)	- 16 MB SPI NOR Flash (data logging) [[Datasheet]](https://docs.rs-online.com/7d70/0900766b81703faf.pdf)
- MB85RS64VPNF‑G‑JNE1	- 64 Kbit SPI FRAM (parameter storage)	[[Datasheet]](https://www.ramxeed.com/assets/images/products/datasheet/FeRAM/s4/MB85RS64V-DS6v1-E.pdf)

Communication :
- USB3300‑EZK	- USB 2.0 High‑Speed PHY (ULPI)	[[Datasheet]](https://ww1.microchip.com/downloads/en/DeviceDoc/00001783C.pdf)
- CP2102N‑A02‑GQFN28 (or CP2102)	- USB‑to‑UART bridge (IO debug console) [[Datasheet]](https://www.silabs.com/documents/public/data-sheets/cp2102n-datasheet.pdf)
- SN65HVD230QD	- 3.3 V CAN transceiver (×2)	[[Datasheet]](https://www.ti.com/lit/ds/symlink/sn65hvd230.pdf)
- TJA1051 - CAN Tranceiver [[datasheet]](https://www.nxp.com/docs/en/data-sheet/TJA1051.pdf)

Power :
- TPS62133RGTR - 3 A step‑down converter (5 V → 3.3 V)	[[Datasheet]](https://www.ti.com/lit/ds/symlink/tps62133.pdf)
- LP2985‑33DBVR	- Low‑noise 3.3 V LDO (sensor supply)	[[Datasheet]](https://www.ti.com/lit/ds/symlink/lp2985.pdf)
- INA226AIDGSR - I²C current/voltage/power monitor (dual battery inputs)	[[Datasheet]](https://www.ti.com/lit/ds/symlink/ina226.pdf)
- MCP73831T‑2ACI/OT	- Li‑Poly charger for the RTC backup battery	[[Datasheet]](https://ww1.microchip.com/downloads/en/DeviceDoc/MCP73831-Family-Data-Sheet-DS20001984H.pdf)

Other :
- PCA9306DCUR	- Dual bidirectional I²C level shifter (3.3 V ↔ 5 V)	[[Datasheet]](https://www.ti.com/lit/ds/symlink/pca9306.pdf)
- WS2812B‑2020 - Addressable RGB LED (status indicator)	[[Datasheet]](https://cdn-shop.adafruit.com/datasheets/WS2812B.pdf)

Connector :
- Hirose DF40C-100DP-0.4V(51) : 100pin - X1 FMU-side
- Hirose DF40C-100DS-0.4V(51) : 100pin - X1 Baseboard-side
- Hirose DF40C-100DP-0.4V(51) : 50pin - X2 FMU-side : 
- Hirose DF40C-100DS-0.4V(51) : 50pin - X2 Baseboard-side 
- MEM2077 - Micro-SD Socket : https://www.lcsc.com/datasheet/C5352762.pdf

The open hardware design of Pixracer (based on FMUv4) is provided [here]{https://github.com/AUAV-OpenSource/FMUv4-PixRacer)
[FMUv5 reference design pinout :](https://docs.google.com/spreadsheets/d/1-n0__BYDedQrc_2NHqBenG1DNepAgnHpSGglke-QQwY/edit#gid=912976165)
