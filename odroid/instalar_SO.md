# Instalación de Ubuntu en Odroid XU4



## Requisitos



- Odroid XU4

- Tarjeta microSD o eMMC

- Adaptador USB

![Odroid](../images/diagram2.png)


## Descarga de imagen



Descargar una versión compatible de Ubuntu para [Odroid XU4](https://odroid.in/ubuntu_16.04lts/), ya que no esta disponible la versión oficial, se descarga una versión compartible ubuntu-16.04.3-4.9-mate-odroid-xu4-20171025.img.xz 



## Grabación de imagen

primero se descomprime la imagen usando:


```
unxz ubuntu-16.04.3-4.9-mate-odroid-xu4-20171025.img.xz
```

(si no lo tienen lo pueden instalar con "sudo apt-get unxz")


si tienes el adaptador de eMMC a microSD debes identificar como la reconoce el sistema ejemplo: mmcblk0 mmcblk0p1 mmcblk0p2 mmcblk0p3



Linux:


```bash
sudo dd if=ubuntu.img of=/dev/mmcblk0p1 bs=4M status=progress
```


## Tambien puedes usar Balena Etcher



1\. Selecciona la imagen.

2\. Selecciona la microSD (identificador).

3\. Selecciona Flash.

4\. Verifica que se instalo correctamente.



## Actualización



```bash
sudo apt update
sudo apt upgrade -y
```



Recuarda para esta versión el usuario y el password es: **odroid**
