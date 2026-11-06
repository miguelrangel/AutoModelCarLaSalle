\# Instalación de ROS Kinetic



\## Agregar repositorios



```bash

sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu xenial main" > /etc/apt/sources.list.d/ros-latest.list'

```



\## Llaves



```bash

sudo apt install curl # if you haven't already installed curl

curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -

```



\## Instalación



```bash

sudo apt update



sudo apt install ros-kinetic-desktop-full

```



\## Environment setup



```

echo "source /opt/ros/kinetic/setup.bash" >> \~/.bashrc

source \~/.bashrc



```



\## Dependencies for building packages



```

sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential 





```



\## Initialize rosdep



```

sudo apt install python-rosdep



```



```

sudo rosdep init

rosdep update



```



\## Create a ROS Workspace



```

source /opt/ros/kinetic/setup.bash

```





```

mkdir -p \~/catkin\_ws/src



```





```

cd \~/catkin\_ws/

```



```

catkin\_make

```



```

source /opt/ros/kinetic/setup.bash

```





\## Make sure ROS\_PACKAGE\_PATH environment variable includes the directory you're in



```

echo "source \\\~/catkin\_ws/devel/setup.bash" >> \\\~/.bashrc

source \\\~/.bashrc

```















