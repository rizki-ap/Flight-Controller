**Hardware Design** 

pixhawk 5x standard :
- specs : https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-011%20Pixhawk%20Autopilot%20v5X%20Standard.pdf
- Bus : https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-010%20Pixhawk%20Autopilot%20Bus%20Standard.pdf
- connector : https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-009%20Pixhawk%20Connector%20Standard.pdf
- 

Component :
Processor 
- STM32F765x microcontroller https://www.st.com/resource/en/datasheet/stm32f765ii.pdf
- STM32f103x microcontroller https://www.st.com/resource/en/datasheet/stm32f103c8.pdf

IMU/Gyro
- ICM‑20689 (×2)	3‑axis gyro + 3‑axis accel, SPI-if https://invensense.tdk.com/wp-content/uploads/2020/03/DS-000114-ICM-20689-v1.3.pdf	
- ICM‑42688‑P https://invensense.tdk.com/download-pdf/icm-42688-p-datasheet/ 
- BMI088 https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bmi088-ds001.pdf

- MS5611‑01BA03	High‑resolution barometric pressure sensor (I²C/SPI)	MS5611 Datasheet
- Magnetometer (Internal)
- IST8310	3‑axis magnetometer (I²C)	IST8310 Datasheet

- W25Q128JVSIM (or JVSIQ)	16 MB SPI NOR Flash (data logging)	W25Q128JV Datasheet
- MB85RS64VPNF‑G‑JNE1	64 Kbit SPI FRAM (parameter storage)	MB85RS64V Datasheet

- USB3300‑EZK	USB 2.0 High‑Speed PHY (ULPI)	USB3300 Datasheet
- CP2102N‑A02‑GQFN28 (or CP2102)	USB‑to‑UART bridge (IO debug console)	CP2102N Datasheet
- SN65HVD230QD	3.3 V CAN transceiver (×2)	SN65HVD230 Datasheet

- TPS62133RGTR	3 A step‑down converter (5 V → 3.3 V)	TPS62133 Datasheet
- LP2985‑33DBVR	Low‑noise 3.3 V LDO (sensor supply)	LP2985 Datasheet
- INA226AIDGSR (×2)	I²C current/voltage/power monitor (dual battery inputs)	INA226 Datasheet
- MCP73831T‑2ACI/OT	Li‑Poly charger for the RTC backup battery	MCP73831 Datasheet

- PCA9306DCUR	Dual bidirectional I²C level shifter (3.3 V ↔ 5 V)	PCA9306 Datasheet
- WS2812B‑2020	Addressable RGB LED (status indicator)	WS2812B Datasheet
