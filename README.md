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

## USAGE
- Instalation ROS2 
- Instalation Micro ROS
