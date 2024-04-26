# IMU_BNO055_PlatformIO
This is Micro ROS project to get data IMU from BNO055 accelerometer, gyroscope and geomagnetic from BOSCH sensortech. This project is running on ROS2 with Distro Humble, for firmware using PlatformIO, for microcontroller using ESP32 and Connected to BNO055 via I2C. To Communication with ROS Computer, in schematic the are USB to Serial(FTDI231). You need to program the FTDI to set fix PID and VID. In ROS Computer need to Register UDEV Device, So we can set Static Port Name of the PCB. 

## Prepare The PCB
- You can find the [gerber](https://github.com/juarendra/IMU_BNO055_MICRO_ROS_HUMBLE_ESP32_PlatformIO/blob/main/SCH/GERBER_IMU_BNO055_BMP280.zip) file on SCH folder, you can Print it to PCB Fabrication Manufacturer like [JLCPCB](https://jlcpcb.com).
<p align="center">
  <img src="DOC/HARDWARE/hw1.png" width="100%" height="100%">
</p>
- This is how look like the PCB based on the gerber file.
- then you can assembly the PCB with Component on this [BOM](https://github.com/juarendra/IMU_BNO055_MICRO_ROS_HUMBLE_ESP32_PlatformIO/blob/main/SCH/ros2_imu.xlsx)

## USAGE
- Instalation ROS2 
- Instalation Micro ROS
