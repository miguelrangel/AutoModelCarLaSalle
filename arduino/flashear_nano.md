# Programación del Arduino Nano

## Software requerido download Arduino IDE 2.0.0 (validado)


En la documentación te sugiere una versión diferente pero se valido con esta versión y funciono bien: [Arduino IDE](https://github.com/arduino/arduino-ide/releases?page=2)


## Check port


```bash
ls /dev/ttyUSB\*
```

o 

```bash
ls /dev/ttyAM\*
```


## Configuración

De la carpeta arduino/firmware **Copy the libraries (MPU6050, I2Cdev,Adafruit_NeoPixel) to the arduino-2.0.0/libraries folder.**


Board:



```bash
Arduino Nano
```



Processor:
```bash
ATmega328P (Old Bootloader)
```


## Compilar

Abrir:

```bash
AutoModelCarLaSalle\docs\arduino\firmware\main
```

Seleccionar: **main.ino**

```text
Verificar que no tenga errores
```


Posteriormente:
```text
Compilar y grabarlo en el arduino nano
```
## Validar con el monitor Serie

Recuerda que esta a **115200** baudios y debe regresar:

```text
 YPR [valor]
```

