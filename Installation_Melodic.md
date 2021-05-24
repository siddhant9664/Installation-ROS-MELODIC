# Installation of ROS (ROBOT OPERATING SYSTEM)
## For installation of ROS MELODIC you must be on UBUNTU version 18.04 only.
### Follow the instructions  [here](https://www.youtube.com/watch?v=gPCxQNQYk2s) (Video Tutorial) or [here](https://itsfoss.com/dual-boot-hdd-ssd/) (Webpage) for detailed Ubuntu 18.04 Installation.
## 1. ROS
#### You can proceed with the instructions provided below or you can find these installation instructions [here](http://wiki.ros.org/melodic/Installation/Ubuntu)
Open a new terminal and execute the commands below.
#### Setup your sources.list
    sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
#### Set up your keys
    sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
#### Update packages and install ROS
	sudo apt update
	sudo apt install ros-melodic-desktop-full
#### Setup the environment
	echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
	source ~/.bashrc	
#### Dependencies
	sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
#### Rosdep
	sudo apt install python-rosdep
	sudo rosdep init
	rosdep update

### 2. Set Up Catkin workspace


```
sudo apt-get install python3-wstool python3-rosinstall-generator python3-catkin-lint python3-pip python3-catkin-tools
pip3 install osrf-pycommon
```

```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws
catkin init
```    


