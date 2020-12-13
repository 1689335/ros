
sh -c 'echo "deb https://mirrors.ustc.edu.cn/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

apt-get update

桌面完整版: (推荐) : 包含ROS、rqt、rviz、机器人通用库、2D/3D 模拟器、导航以及2D/3D感知
sudo apt-get install ros-kinetic-desktop-full
或者 点这里
｀｀｀
桌面版安装: 包含ROS、rqt、rviz以及通用机器人函数库。
sudo apt-get install ros-kinetic-desktop
或者 点这里

基础版安装: (简版) 包含ROS核心软件包、构建工具以及通信相关的程序库，无GUI工具。
sudo apt-get install ros-kinetic-ros-base
或者 点这里

单个软件包安装: 你也可以安装某个指定的ROS软件包（使用软件包名称替换掉下面的PACKAGE）:
sudo apt-get install ros-kinetic-PACKAGE
例如：
sudo apt-get install ros-kinetic-slam-gmapping
要查找可用软件包，请运行：

apt-cache search ros-kinetic
｀｀｀

sudo rosdep init
rosdep update

echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc



apt-get install python-rosinstall python-rosinstall-generator python-wstool build-essential
