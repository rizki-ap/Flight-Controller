**Hardware Design** 

pixhawk 5x standard :
- specs : https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-011%20Pixhawk%20Autopilot%20v5X%20Standard.pdf
- Bus : https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-010%20Pixhawk%20Autopilot%20Bus%20Standard.pdf
- connector : https://github.com/pixhawk/Pixhawk-Standards/blob/master/DS-009%20Pixhawk%20Connector%20Standard.pdf
- 

Component :
Processor 
- STM32F765x microcontroller [[datasheet]](https://www.st.com/resource/en/datasheet/stm32f765ii.pdf)
- STM32f103x microcontroller [[datasheet]](https://www.st.com/resource/en/datasheet/stm32f103c8.pdf)

Sensors :
- ICM‑20689 (×2)	3‑axis gyro + 3‑axis accel, SPI-if [[datasheet]](https://product.tdk.com/system/files/dam/doc/product/sensor/mortion-inertial/imu/data_sheet/ds-000143-icm-20689-datasheet.pdf)
- ICM‑42688‑P [[datasheet]](https://invensense.tdk.com/download-pdf/icm-42688-p-datasheet/)
- BMI088 [[datasheet]](https://www.bosch-sensortec.com/media/boschsensortec/downloads/datasheets/bst-bmi088-ds001.pdf)
- MS5611‑01BA03	High‑resolution barometric pressure sensor (I²C/SPI)	[[Datasheet]](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=showdoc&DocId=Data+Sheet%257FMS5611-01BA03%257FB3%257Fpdf%257FEnglish%257FENG_DS_MS5611-01BA03_B3.pdf)
- Magnetometer (Internal)
- IST8310	3‑axis magnetometer (I²C)	[[Datasheet]](http://www.isentek.com/en/dlf.php?file=../sensor_datasheet/IST8310%2520Datasheet%2520v1.2.pdf)

Memory :
- W25Q128JVSIM (or JVSIQ)	16 MB SPI NOR Flash (data logging) [[Datasheet]](https://www.winbond.com/resource-files/w25q128jv_dtr%2520revb%252007202016.pdf)
- MB85RS64VPNF‑G‑JNE1	64 Kbit SPI FRAM (parameter storage)	[[Datasheet]](https://www.fujitsu.com/downloads/MICRO/fsa/pdf/products/memory/fram/DS_MB85RS64V-DS501-00005-4v0-E.pdf)

Communication :
- USB3300‑EZK	USB 2.0 High‑Speed PHY (ULPI)	[[Datasheet]](https://ww1.microchip.com/downloads/en/DeviceDoc/00001783C.pdf)
- CP2102N‑A02‑GQFN28 (or CP2102)	USB‑to‑UART bridge (IO debug console)	CP2102N Datasheet
- SN65HVD230QD	3.3 V CAN transceiver (×2)	SN65HVD230 Datasheet

Power :
- TPS62133RGTR	3 A step‑down converter (5 V → 3.3 V)	TPS62133 Datasheet
- LP2985‑33DBVR	Low‑noise 3.3 V LDO (sensor supply)	LP2985 Datasheet
- INA226AIDGSR (×2)	I²C current/voltage/power monitor (dual battery inputs)	INA226 Datasheet
- MCP73831T‑2ACI/OT	Li‑Poly charger for the RTC backup battery	MCP73831 Datasheet

- PCA9306DCUR	Dual bidirectional I²C level shifter (3.3 V ↔ 5 V)	PCA9306 Datasheet
- WS2812B‑2020	Addressable RGB LED (status indicator)	WS2812B Datasheet
