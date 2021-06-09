# ROS Environment
## SBG_driver
ROS driver package for communication with the SBG navigation systems. [Github link](https://github.com/SBG-Systems/sbg_ros_driver)
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
MAVLink extendable communication node for ROS with proxy for Ground Control Station. [Github link](https://github.com/mavlink/mavros)
- Command
  ```
  roslaunch mavros apm2.launch fcu_url:="udp://:14550@:14550"
  ```

## udp com
It provides ROS Services for creating sockets, sending and receiving UDP data. [Github link](https://github.com/continental/udp_com)
- Command
  ```
  roslaunch udp_com udp_com.launch
  rosservice call /eth1/udp/create_socket "srcAddress: '0.0.0.0'
  destAddress: '0.0.0.0'
  port: 1600
  isMulticast: false"

  ```

## ROS bag files containing sensor data
- [IMU + GNSS](../../data/rosbag/sbg_driver)
- [MAVROS](../../data/rosbag/mavros)
- [UDP Com (SBES)](../../data/rosbag/udp_com)
