FROM ros:melodic-ros-base-bionic

RUN apt update
RUN apt install curl gnupg2 lsb-release -y
RUN curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | apt-key add -
RUN sh -c 'echo "deb [arch=$(dpkg --print-architecture)] http://packages.ros.org/ros2/ubuntu $(lsb_release -cs) main" > /etc/apt/sources.list.d/ros2-latest.list'

RUN apt update
RUN apt install ros-crystal-ros-base -y
RUN apt install python3-argcomplete -y
