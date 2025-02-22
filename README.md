# IMU_BNO055_PlatformIO
This is Micro ROS project to get data IMU from BNO055 accelerometer, gyroscope and geomagnetic from BOSCH sensortech. This project is running on ROS2 with Distro Humble, for firmware using PlatformIO, for microcontroller using ESP32 and Connected to BNO055 via I2C. To Communication with ROS Computer, in schematic the are USB to Serial(FTDI231). You need to program the FTDI to set fix PID and VID. In ROS Computer need to Register UDEV Device, So we can set Static Port Name of the PCB. 

## Prepare The PCB
- There are PCBs that have been made based on existing requirements. 
- You can find the [gerber](https://github.com/juarendra/IMU_BNO055_MICRO_ROS_HUMBLE_ESP32_PlatformIO/blob/main/SCH/GERBER_IMU_BNO055_BMP280.zip) file on SCH folder, you can Print it to PCB Fabrication Manufacturer like [JLCPCB](https://jlcpcb.com).
<p align="center">
  <img src="DOC/HARDWARE/hw1.png" width="50%" height="50%">
  <img src="DOC/HARDWARE/hw2.png" width="50%" height="50%">
</p>

- This is how look like the PCB based on the gerber file.
- Then you can assembly the PCB with Component on this [BOM](https://github.com/juarendra/IMU_BNO055_MICRO_ROS_HUMBLE_ESP32_PlatformIO/blob/main/SCH/BOM_IMU_BNO055_BMP280.csv).
- Once the assembly is complete you will see it as shown in the image below 
<p align="center">
  <img src="DOC/HARDWARE/hw7.png" width="50%" height="50%">
</p>

## Spesification
Based on the PCB that has been made and assembled, you will get a module with the following specifications:
- ESP32 WROOM
- USB TYPE C
- FT231 as USB Proggrammer
- BNO055
- BMP280
- Modul charger tp4056 for Charger Lipo Batt
- Switch On OFF
- SD Card as save Data Loging

## Program VID and PID USB to Serial 
this procedure is  for WINDOWS only:
- Download and Install FT prog Software on [this link](https://ftdichip.com/utilities/#ft_prog)
- Open FT Prog
- Connect module to PC 
- Click on Loupe icon, then your device is auto detected
- On Tab USB Device Decription you will see PID and VID Form
- You can change it with your custom value.
- Flash it to eeprom on your device

## Flash the Firmware with  Platformio 
## USAGE
- Instalation ROS2 
- Instalation Micro ROS
- run Micro ros with the predefined port name
- You can find several topics that will be published as in the table below
