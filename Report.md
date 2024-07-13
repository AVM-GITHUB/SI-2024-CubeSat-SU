![image](https://github.com/user-attachments/assets/d0aab0e4-ad3b-482b-9978-4dbb1321aaa1)


# Abstract


# Introduction

# CubeSat Basics

![image](https://github.com/user-attachments/assets/51c24b77-14a1-479f-a7d5-bf422833fb5b)

**What is a CubeSat ?**

A CubeSat, short for Cube Satellite, is a type of miniaturized satellite used primarily for space research, education, and commercial purposes. The term "CubeSat" refers to a standard for small satellites that was developed to reduce the cost of satellite missions and facilitate easier access to space.

**Charecteristics of CubeSat**

Standardized Size and Shape: CubeSats are typically small, cube-shaped satellites with standardized dimensions. The most common size is 10 cm x 10 cm x 10 cm (1U), but they can also be larger configurations such as 1.5U, 2U, 3U, and so on, where each "U" represents a unit of 10 cm x 10 cm x 10 cm.

Modular Design: CubeSats are designed to be modular, which means they can be easily customized and assembled using standardized components and interfaces. This modularity allows for rapid development and deployment of satellite missions.

Low Cost: By using off-the-shelf components and leveraging the small size, CubeSats are significantly cheaper to build and launch compared to traditional larger satellites. This affordability has democratized access to space for universities, small companies, and even individual researchers.
This feauture of CubeSat allows for mass modular production and low cost production. 

Short Development Cycles: CubeSats typically have shorter development cycles compared to larger satellites, which allows for quicker iteration and testing of new technologies and experiments in space.

Payload Flexibility: Despite their small size, CubeSats can carry a variety of payloads depending on the mission objectives. Payloads can include scientific instruments, cameras, communication systems, and more. But as compared to traditional satellites the working aspect of a CubeSat is not much diverse and is limited due to its smaller size .

**CubeSat Dispenser System**

A dispenser is an interface between CubeSat and  Launch vehicle . 

![image](https://github.com/user-attachments/assets/76469eaf-3984-470e-90c6-208ed10a1add)

During the launch, the CubeSats are fully enclosed by the dispensers and are only dispensed upon the signal by the launch vehicle.

**Launch Vehicles (LVs) or, Rockets.**

# Satellite Communication

## Basic Digital Modulation
-Modulation is the process of superimposing high-frequency carrier signals with low-frequency message signals resulting in a modulated wave. In modulation, one of the three parameters of the carrier wave is changed i.e. amplitude, frequency or phase according to the amplitude of the message signal at a given time instant. It is an important technique used to increase the range of communication, increase the signal-to-noise ratio, and decrease the size of the antenna.

In Digital Modulation, only the carrier signal is analogue and the message signal is in digital form.
**Some terms used in Digitial Modulation are :**

**Amplitude Shift Keying  :** 


![image](https://github.com/user-attachments/assets/1b14ba58-6beb-4a89-b2f7-fa62804a94e7)

**Frequency Shift Keying  :**
In Frequency Shift Keying (FSK), each symbol in the message signal gives a unique frequency to the carrier wave. There are two types of FSK, Binary and M-ary. In Binary FSK, logic 1 is associated with certain frequency of carrier wave e.g. 50MHz and logic 0 is associated with different frequency other than 50MHz e.g. 25MHz. In M-ary FSK, a group of log2M bits are considered together rather than 1 bit at a time and the frequency is associated with this group of bits.

![image](https://github.com/user-attachments/assets/7eece47d-a9f3-415a-a40e-73d52dba83f6)

Block Diagram of Frequency shift keying 

![image](https://github.com/user-attachments/assets/af9a20a3-ff6f-4566-b315-8ec5bcf63f88)

**Phase Shift Keying  :**

Phase-shift keying is a digital modulation process which conveys data by changing the phase of a constant frequency carrier wave. The modulation is accomplished by varying the sine and cosine inputs at a precise time.

![image](https://github.com/user-attachments/assets/51c04203-0783-4f67-8d0e-58457f7b37f3)


## Basic Bandpass Modulation

## ELectromagnetic Specturm

## Satellite Orbit Fundamentals

## LoRa Tranceiver (Radio) Architecture

![image](https://github.com/user-attachments/assets/50edf3dd-8217-4afc-9fad-5277fabf98fe)

-LoRa Basics 

## Antennas

-Antenna Basics
  
**Why do we need different type of antennas ?**
Because there are many applications involving radio, the way the radio wave should be transmitted, received and propagated will vary depending on the application requirements. This makes the antenna a critical component in any communication system, so it is important for the user to select the correct type of antenna. There is no point in investing in a good performance radio and then forgetting about the antenna.

**Types of Antennas :**

**Standard Dipole**


A variation of this type of antenna is 'V' (or "Vee") antenna is a dipole with a bend in the middle so its arms are at an angle instead of co-linear.

**Whip/Monopole**
A monopole antenna is a class of radio antenna consisting of a straight rod-shaped conductor, often mounted perpendicularly over some type of conductive surface, called a ground plane. 
However at lower frequencies, the size of the dipole can become impractical.

![image](https://github.com/user-attachments/assets/db58de2b-f904-4862-b3b4-1bd7e40a2d05)

**Yagi-Uda**



## Lab Excercises

## Introduction ot ESP32 Development Board

## ESP32+LoRa

-By integrating ESP32 with LoRa we get a versatile platform capable of connecting to the internet via Wi-Fi while also transmitting data over long distances using LoRa. This makes it ideal for applications like sensor networks, remote monitoring, and other IoT projects where both local and long-range communication are required. 


**Lab-1 : Introduction to ESP32 Programming**
 
**Lab-2 : Intro to GPIO programming**

**Lab-3 : Dimming LED using PWM**

**Lab-4 : Dimming multiple LEDs**

**Lab 5: Printing data in the serial monitor**

**Lab 6: Controlling an LED through serial monitor**

**Lab 7: I2C-based OLED Display control**

**Lab 8: Introduction Signal Processing using Python**

**Lab 9: I2C temperature sensor interface**

**Lab 10: Introduction to LoRa module**

**Lab 11: LoRa communication**

**Lab 12: Communication between two LoRa nodes**

**Lab 13: LoRa one-to-many communication setup**

**Lab 14: Introduction to antenna modeling and simulation software 4NEC2.**

**Lab 15: Physical design of Dipole and V-dipole antennas**

**Lab 16: Introduction to TinyGS**

**Lab 17: Setting up a TinyGS ground station**



# Setting up TinyGS groundstation
