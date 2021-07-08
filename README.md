# MOVE-THE-ARM_AI-PART

لإستعلام نظام رزو في التحكم بحركة الذراع نحتاج إلى تثبيت متصفح افتراضي ثم تنزيل نظام ابونتو 
وذلك سيتم بعدة أوامر متسلسلة 

رابط تحميل Virtual Box
https://www.virtualbox.org/wiki/Downloads


صفحة أوامر الذراع الآلية
https://s-m.com.sa/ros.txt


أولاً: تثبيت نظام الروز على ابنتو باستخدام الاأوامر التالية:

$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
$ sudo apt-get update


ثانيًا: أوامر لتثبيت الروز (إصدار كاينتك):

$ sudo apt-get install ros-kinetic-desktop-full
$ apt-cache search ros-kinetic
$ echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc


ثالثًا: أوامر لتثبيت لغة بايثون:

$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
$ sudo apt install python-rosdep
$ sudo rosdep init
$ rosdep update
$ sudo apt-get install ros-noetic-catki
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/


:رابعًا: تنظيم انزال بكج الذراع 

$ rosdep install --from-paths src --ignore-src -r -y
$ sudo apt-get install ros-kinetic-moveit
$ sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui
$ sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control
$ sudo nano ~/.bashrc
