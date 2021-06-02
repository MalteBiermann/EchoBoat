FROM ros:melodic-ros-base-bionic

# install ros package
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654 && \
	apt-get update && \
	apt-get install -y --no-install-recommends \
	ros-melodic-robot=1.4.1-0* \
	ros-melodic-nmea-navsat-driver \
	ros-melodic-nmea-comms \
	ros-melodic-mavros \
	ros-melodic-sbg-driver \
	ros-melodic-udp-com && \
	/opt/ros/melodic/lib/mavros/install_geographiclib_datasets.sh && \
	rm -rf /var/lib/apt/lists/*
