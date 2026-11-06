# Instalación de Intel RealSense SR300


Cuando ya tenga instalado ROS Kinetic es suficiente con el siguiente comando:


```
sudo apt install ros-kinetic-librealsense2\*
```





**otra forma no recomendada para ejecutar en la Odroid**





## Dependencias



```bash
sudo apt update
sudo apt install git cmake libusb-1.0-0-dev
```



## Clonar librealsense



```bash
git clone https://github.com/IntelRealSense/librealsense.git
cd librealsense
mkdir build
cd build
```



## Compilar



```bash
cmake ..
make -j4
sudo make install
```



## Verificación



```bash
realsense-viewer
```

