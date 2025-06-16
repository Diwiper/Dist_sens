
# Ultrasonic Distance Meter with OLED Display (STM32)

This project measures the distance to an object using an HC-SR04 ultrasonic sensor and displays it on a 0.96" I2C OLED screen (SSD1306) using an STM32F103C8T6 microcontroller.

## Features

- Real-time distance measurement
- I2C communication with OLED
- Code written using STM32 HAL
- Display update every 100–300 ms

##  Hardware

- STM32F103C8T6 (Blue Pill)
- HC-SR04 ultrasonic sensor
- OLED 128x64 (I2C, SSD1306)
- ST-Link programmer

## Pinout

| Component | Pin on STM32 |
|----------|--------------|
| HC-SR04 Trig | PA9 |
| HC-SR04 Echo | PA8 |
| OLED SDA | PB7 |
| OLED SCL | PB6 |

## How It Works

The microcontroller triggers the ultrasonic sensor, receives the echo, calculates the distance using the speed of sound, and then prints the result to the OLED display.
