# Control Robot Arm - AI PART

لإستعلام نظام روز في التحكم بحركة الذراع نحتاج أولاً لتثبيت برنامج- virtual Box

ثانيًا تثبيت نظام ابونتو على البرنامج الذي قمنا بتثبيته مسبقًا- Ubuntu 16.04 




* ### رابط تحميل Virtual Box
```
https://www.virtualbox.org/wiki/Downloads
```

* ### رابط تحميل Ubuntu 16.04
```
https://releases.ubuntu.com/16.04/
```


# First
أولاً: تثبيت نظام الروز على ابنتو باستخدام الأوامر التالية:
* ### صفحة أوامر الذراع الآلية
```
https://s-m.com.sa/ros.txt
```
```
$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

$ sudo apt-get update
```

# Second
ثانيًا: أوامر لتثبيت الروز (إصدار كاينتك):
```
$ sudo apt-get install ros-kinetic-desktop-full

$ apt-cache search ros-kinetic

$ echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

# Third
ثالثًا: أوامر لتثبيت لغة بايثون:
```
$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

$ sudo apt install python-rosdep

$ sudo rosdep init

$ rosdep update

$ sudo apt-get install ros-noetic-catki

$ mkdir -p ~/catkin_ws/src

$ cd ~/catkin_ws/
```


# Fourth
:رابعًا: تنظيم انزال بكج الذراع 
```
$ rosdep install --from-paths src --ignore-src -r -y

$ sudo apt-get install ros-kinetic-moveit

$ sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

$ sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

$ sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

$ sudo nano ~/.bashrc
```



![1](https://user-images.githubusercontent.com/86114919/125003372-bfd73880-e05f-11eb-9007-6ead9918e109.png)







