# Flashing the Arduino Nano

## Required software

Download and install Arduino IDE 2.0.0, which has been tested and validated for this project:

[Arduino IDE](https://github.com/arduino/arduino-ide/releases?page=2)

Although the official documentation recommends a different version, Arduino IDE 2.0.0 has been tested successfully.

## Checking the serial port

Check which serial port is assigned to the Arduino:

```bash
ls /dev/ttyUSB\*
```

Alternatively, check:

```bash
ls /dev/ttyAM\*
```


## Configuration

From the `arduino/firmware` folder, copy the following libraries to the `arduino-2.0.0/libraries` folder:

**MPU6050, I2Cdev, and Adafruit_NeoPixel**

Select the following board:

```text
Arduino Nano
```

Select the following processor:
```bash
ATmega328P (Old Bootloader)
```


## Compiling and uploading the firmware

Open the following sketch:

```bash
AutoModelCarLaSalle\docs\arduino\firmware\main
```

Select **main.ino** and verify that it compiles without errors.

Then compile the sketch and upload it to the Arduino Nano.

## Verifying the firmware with the Serial Monitor

Open the Serial Monitor and set the baud rate to **115200**. The Arduino should output:

```text
YPR [value]
```