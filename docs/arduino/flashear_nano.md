\# Programación del Arduino Nano



\## Software requerido



\- Arduino IDE 1.8.x

\## Download Arduino IDE 2.0.0 (validado)





En la documentación te sugiere una versión diferente pero se valido con esta versión y funciono bien: \[Arduino IDE]{https://github.com/arduino/arduino-ide/releases?page=2}





\## Check port



```

ls /dev/ttyUSB\*

```

o 

```

ls /dev/ttyAM\*

```







\## Configuración

** Copy the libraries (MPU6050, I2Cdev,Adafruit_NeoPixel) to the arduino-2.0.0/libraries folder.**


Board:



```

Arduino Nano

```



Processor:



```

ATmega328P (Old Bootloader)

```



\## Compilar



Abrir:



```

AutoModelCarLaSalle\docs\arduino\firmware\main
```



Seleccionar: main.ino



```text

Verificar que no tenga errores

```



Posteriormente:



```text

Subir

```



\## Validar con el monitor Serie

115200 baudios debe regresar:

```text

 YPR [valor]

```

