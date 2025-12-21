# Smart-Timer-For-Mosquito-Repellent
A timer circuit project to save energy using embedded logic
A basic embedded system project to control the ON/OFF cycle of a liquid mosquito repellent for energy saving.

My mini project is an automatic, time-based mosquito repellent system. In normal repellents, people often forget to switch them ON or OFF, which wastes liquid, electricity, and causes unnecessary chemical exposure. My system solves this by working only during mosquito-active hours, making it energy-efficient, safe, and convenient. It uses a microcontroller as the brain, a relay to control the repellent, and a real-time clock module to track time. The microcontroller runs a program that automatically switches the repellent ON and OFF

## 🔧 Tools Used:

* Software Tools

 Arduino IDE:
Used to write, compile, and upload the embedded C program.
Arduino Compiler:
Converts embedded C code into machine code.
Embedded C Language:
Used for programming the microcontroller.

## Components Used
Component	Purpose
Microcontroller (e.g., Arduino/PIC)	Brain of the system; controls timing and relay
Relay	Acts as a switch to turn the mosquito repellent ON/OFF
Real-Time Clock (RTC) Module	Keeps track of current time to operate only during mosquito-active hours
Power Supply	Powers the microcontroller, RTC, and relay
Mosquito Repellent	The device being controlled (liquid or electric)


## Working Flow Diagram

<img width="769" height="473" alt="image" src="https://github.com/user-attachments/assets/4b0bf5d2-fcf1-4aad-b585-a68c963aa1ef" />



1. Power ON

System is powered via the power supply. MCU, RTC, relay, and optional buzzer are energized.

2.RTC Sends Time

The RTC module continuously keeps track of real-time.

It sends the current time (hours, minutes, seconds) to the microcontroller via I2C/SPI communication.

3.Microcontroller Processes Time

MCU reads the time from RTC.

Compares it with pre-set mosquito-active hours (e.g., 6 PM – 6 AM).

4.Decision Making

If current time is within active hours:

MCU sends HIGH signal to relay → turns repellent ON.

Optional: MCU triggers buzzer to indicate repellent is active.

If current time is outside active hours:

MCU sends LOW signal to relay → turns repellent OFF.

Optional: Buzzer can beep briefly to indicate OFF.

5.Relay Operates Repellent

Relay switches the main power of mosquito repellent ON/OFF based on MCU signal.

6.Continuous Loop

MCU continuously monitors time from RTC and repeats the ON/OFF process automatically without user intervention










## ✅ Features:
- Automatic timer cycle
- 30% energy efficiency
