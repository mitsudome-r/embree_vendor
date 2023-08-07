ARG ROS_DISTRO=humble
FROM ros:${ROS_DISTRO} as build-stage
RUN 
RUN apt-get update && \
    DEBIAN_FRONTEND=noninteractive \
    apt-get install -y \
    python3-bloom fakeroot dpkg-dev debhelper wget apt-utils\
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
