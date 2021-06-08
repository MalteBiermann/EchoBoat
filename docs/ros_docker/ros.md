# ROS Environment
## SBG_driver
ROS driver package for communication with the SBG navigation systems
- Command
  ```
  roslaunch sbg_driver sbg_device.launch
  ```
- Driver Output  
    Topic | Description
    ------|------------
    /imu/data| IMU data  
    /imu/temp| IMU temperature  
    /imu/velocity| IMU velocity data  
    /imu/mag| IMU magnetic field  
    /imu/pres| IMU pressure data  
    /imu/pos_ecef| Earth-Centered Earth_Fixed position  
    /imu/utc_ref| UTC time reference  
    /imu/nav_sat_fix| Navigation satellite  
    /sbg/ekf_euler| SbgEkfEuler  
    /sbg/ekf_nav| SbgEkfNav  
    /sbg/ekf_quat| SbgEkfQuat  
    /sbg/gps_pos| SbgGpsPos  
    /sbg/gps_vel| SbgGpsVel
    /sbg/imu_data| SbgImuData
    /sbg/imu_short| SbgImuShort
    /sbg/mag| SbgMag
    /sbg/mag_calib| SbgMagCalib
    /sbg/odo_vel| SbgOdoVel
    /sbg/ship_motion| SbgShipMotion
    /sbg/utc_time| SbgUtcTime
## MAVROS
MAVLink extendable communication node for ROS with proxy for Ground Control Station
- Command
  ```
  roslaunch mavros apm.launch fcu_url:=udp://localhost
  ```
- Driver Output 

## ROS bag files
- [IMU + GNSS]
