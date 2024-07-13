# Introduction to CubeSat and satellite Communication 

![image](https://github.com/user-attachments/assets/d0aab0e4-ad3b-482b-9978-4dbb1321aaa1)


# Abstract

The report encapsulates the comprehensive learning journey of the Summer Internship 2024 on Introduction to CubeSat and Satellite Communication, providing a deep dive into CubeSat fundamentals, satellite communication principles, LoRa protocol applications, and antenna design. Participants engaged in hands-on experiences including programming ESP32 platforms, configuring TinyGS ground stations, and simulating antenna designs using 4NEC2 software. Led by expert instructors from Silicon University and the Indian Institute of Space Science and Technology, alongside industry guidance from ToSpace, the internship fostered a practical understanding of aerospace technologies. Culminating in a project to design and implement ground stations, participants showcased their skills in a poster presentation, reinforcing their readiness for future endeavors in satellite engineering and space technology.

# Introduction

CubeSat and Satellite Communication offers a structured learning path covering fundamental aspects of embedded systems, communication systems, LoRa technology, antenna design, and the deployment of a TinyGS ground station. Participants begin by mastering ESP32 embedded systems through practical exercises in the Arduino IDE, learning GPIO programming, PWM control for LED dimming, and interfacing with sensors. They then delve into the basics of communication systems, understanding modulation techniques, digital communication principles, and the electromagnetic spectrum.

Next, the course focuses on LoRa basics, exploring spread-spectrum modulation, LoRa radio architecture, and practical implementation using ESP32 with the RA-02 LoRa module. Participants engage in hands-on labs to establish communication between two ESP32 boards equipped with LoRa modules, measuring signal strength and quality using RSSI and SNR metrics.

Antenna fundamentals follow, where participants learn about radiation mechanisms, antenna types, and design principles. Using simulation software like 4NEC2, they simulate antenna configurations, optimizing performance through practical tuning with tools like the NanoVNA. This segment equips participants with essential skills for designing and refining antennas suitable for satellite communication applications.

The culmination of the course involves the deployment of a TinyGS ground station. Participants apply their acquired knowledge to set up and configure ground stations using ESP32 platforms, establishing bidirectional communication with CubeSats or other satellites. Through collaborative project work, they demonstrate proficiency in satellite communication systems, antenna deployment, and operational management of ground stations, preparing them for real-world applications in the burgeoning field of CubeSats and satellite communication technologies.

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

A Yagi–Uda antenna, or simply Yagi antenna, is a directional antenna consisting of two or more parallel resonant antenna elements in an end-fire array; these elements are most often metal rods (or discs) acting as half-wave dipoles.Yagi–Uda antennas consist of a single driven element connected to a radio transmitter or receiver (or both) through a transmission line, and additional passive radiators with no electrical connection, usually including one so-called reflector and any number of directors

![image](https://github.com/user-attachments/assets/e6d1a00c-76b8-4a16-945b-700e59773cc7)


## Lab Excercises

## Introduction ot ESP32 Development Board

## ESP32+LoRa

-By integrating ESP32 with LoRa we get a versatile platform capable of connecting to the internet via Wi-Fi while also transmitting data over long distances using LoRa. This makes it ideal for applications like sensor networks, remote monitoring, and other IoT projects where both local and long-range communication are required. 


 ## Lab-1 Introduction to ESP32:
<ul>
  <li>Install and configure Arduino IDE</li>
  <li>Introduction to ESP32 development kit.</li>
  <li>Write and execute a C-code to blink an LED on the dev board.</li>
</ul>

-[Datasheet ESP32](https://github.com/silicon-sat/SI-2024-CubeSat/blob/main/docs/Datasheet-ESP32.pdf)

**ESP-32**
The ESP32 is a powerful microcontroller with built-in Wi-Fi and Bluetooth capabilities, ideal for IoT projects. It features:
<ul>
<li>Dual-core processor: Runs at up to 240 MHz.</li>
<li>Low power consumption: Great for battery-operated devices.</li>
<li>Variety of GPIO pins: Supports various interfaces like SPI, I2C, UART, PWM, etc.</li>
<li>Rich development environment: Compatible with Arduino IDE, PlatformIO, and ESP-IDF.</li>

![347949728-5ec3834a-2b5e-4f80-9f7a-1f6c9c4a9648](https://github.com/user-attachments/assets/ed259ecf-81e2-40d7-897c-a7137e76329a)
</ul>


```C
#define LED_BUILTIN 2
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(LED_BUILTIN, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```



## Lab 2: Intro to GPIO programming

In this Lab exercise, students learn to configure a GPIO as an output and control an LED with it.

![esp32-devkit-v1-pinout-imicon-01-copy](https://github.com/user-attachments/assets/5817401d-406e-4832-806f-188978cfb6bd)


-[SOURCE FILE](LED/Aurdino/)

```C
#define LED 2
void setup() {
  // initialize digital pin LED_BUILTIN as an output.
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(LED, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

## Lab -3(Dimming LED using PWM)💡
-In this exercise we used the ESP32 to control the light intensity of an external LED using PWM signal.
From the [LED Datasheet](https://github.com/silicon-sat/SI-2024-CubeSat/blob/main/docs/Datasheet-LED-XLMR01DE.pdf) tabulate the following data:
| parameters | value |
|------------|-------|
|MAX Forward Current|30mA|
|Forward Voltage|1.85V|
|Dominant Wavelength|640nm|
|Colour|Red|
|Total Capacitance|  45pF |
|Operating Range|-45 to 85C|

```c
int led = 13;
int led2 = 2;
int brightness=0;
int fadeAmount=5;

void setup() {
  //initialize digital pin LED_BUILTIN as an output.
  pinMode(led, OUTPUT);
  pinMode(led2, OUTPUT);
 
}

// the loop function runs over and over again forever
void loop() {
 analogWrite(led,brightness);
 analogWrite(led2,brightness);

 brightness=brightness + fadeAmount;

 if( brightness<=0 || brightness>=255 ){
  fadeAmount=-fadeAmount;
 }
 delay(30);
 }
```






## Lab 4: Dimming multiple LEDs💡💡

ESP32 GPIO pins were used to dim multiiple LEDs with different delays.

![d2360516-8034-4558-91b5-4f4b3313295e](https://github.com/user-attachments/assets/816c42e8-678d-4443-aa0a-1899a5a82114)

Parameter for the LED Datashet

| parameters | value |
|------------|-------|
|MAX Forward Current|30mA|
|Forward Voltage|1.85V|
|Dominant Wavelength|640nm|
|Colour|Red|
|Total Capacitance|  45pF |
|Operating Range|-45 to 85C|

```C
#define LED1 2
#define LED2 4
#define LED3 5
#define LED4 18
#define LED5 19

// Array to hold LED pin numbers
int leds[] = {LED2, LED3, LED4, LED5};

// Corresponding delays for each LED
int delays[] = {1000, 700, 100, 500};

void setup() {
  pinMode(LED1, OUTPUT); // LED1 is not used in loop, so just initialized here
  for (int i = 0; i < sizeof(leds) / sizeof(leds[0]); i++) {
    pinMode(leds[i], OUTPUT);
  }
}

void loop() {
  for (int i = 0; i < sizeof(leds) / sizeof(leds[0]); i++) {
    digitalWrite(leds[i], HIGH);
    delay(delays[i]);
    digitalWrite(leds[i], LOW);
    delay(50); // Common delay after each LED blinks
  }
}
```

## Lab 5: Printing data in the serial monitor

-**Serial Monitor** is an essential tool when creating projects with Arduino. It can be used as a debugging tool, testing concepts, or communicating directly with the Arduino board.

-The **Arduino IDE 2** has the Serial Monitor tool integrated with the editor, which means that no external window is opened when using the Serial Monitor. This means that you can have multiple windows open, each with its own Serial Monitor.
```c
#include <Arduino.h>

void setup() {
  // Initialize Serial Monitor
  Serial.begin(115200);
}

void loop() {
  // Print "Hello" to Serial Monitor
  Serial.println("Hello");

  // Delay for 1 second (1000 milliseconds)
  delay(1000);
}

```


## Lab 6: Controlling an LED through serial monitor

Controlling an LED connected to ESP32 by reading commands from the serial monitor and turning the LED on or off based on those commands.

```c
//ESP32 TO serial monitor
#define LED 2

void setup(){
  Serial.begin(9600);
pinMode(LED, OUTPUT);
}

void loop(){
  if(Serial.available()){
    String command = Serial.readStringUntil('\n');
    
    if(command == "ON"){
      digitalWrite(LED, HIGH);
      Serial.println("Turn LED ON ");
    }
    else if (command == "OFF"){
      digitalWrite(LED, LOW);
      Serial.println("Turn LED OFF");

    }
  }

  
}
```

## Lab 7: I2C-based OLED Display control

I2C-based OLED pin details. Importing OLED libraries. Structure of the OLED. Displaying simple Text and Scrolling Text in different ways.

![cc4428ab-5a48-4624-ba07-d3a0e69c871d](https://github.com/user-attachments/assets/20e2e48b-122f-42df-bcb7-cf429225e76f)

```C
#include<SPI.h>
#include<Wire.h>
#include<Adafruit_GFX.h>
#include<Adafruit_SSD1306.h>

#define SCREEN_WIDTH 128 //OLED DISPLAY WIDTH
#define SCREEN_HEIGHT 64
#define OLED_RESET 4
#define SCREEN_ADDRESS 0X3C
Adafruit_SSD1306 display(SCREEN_WIDTH,SCREEN_HEIGHT,&Wire,OLED_RESET);

void setup(){
  Serial.begin(9600);
  if(!display.begin(SSD1306_SWITCHCAPVCC,SCREEN_ADDRESS)){
    Serial.println(F("SSD1306 allocation failed"));
    for(;;);
  }

delay(100);
display.clearDisplay();
display.setTextSize(1);
display.setTextColor(SSD1306_WHITE);
display.setCursor(0,0);
display.println(F("HELLO SILICONITES!!!"));
display.display();
delay(2000);
}
void loop(){}
```




## Lab 8: Introduction Signal Processing using Python
You can use lab1-fft.py and lab2-fsk.py as reference for the following exercises:
Write a python program to create a cosine wave of frequency 2MHz with 256 samples per cycle.
Plot it with proper annonation and axis labeling.
Compute the FFT of the above signal and plot it.
You will notice the FFT resolution is very limited for a single cycle.
Create another a signal of frequency 3MHz, add it to above signal and do FFT for the resultant signal.
Simulate lab2-fsk.py and anlayze the plot to understand FSK modulation.
Change the code such that the modulation frequency for 1 is 4MHz and for 0 it is 3MHz.
Change the above code to simulate ASK modulation.
Add demodulation to the above code and plot the time-domain waveform, as well as the FFT of the demodulated signal.
Add a moving average filter to remove the high-frequency component from the demodulated signal.

### sine wave

![lab-fsk](https://github.com/user-attachments/assets/58df6f40-b9b0-467f-bd31-57e3e06bcbbb)

![fftsin](https://github.com/user-attachments/assets/b73f870f-4485-4439-9b65-15f2b836a168)

```py
import numpy as np
import matplotlib.pyplot as plt

#Parameters
f_signal = 2e6  # 2 MHz signal frequency
fs = 0.5e9     # Sampling frequency (0.5 GHz)
num_samples = 256  # Number of samples
total_time = 500e-9  # Total time duration (500 ns)
time_period = 0.5e-6  # Time period of the signal (0.5 microseconds)

#Time vector
t = np.linspace(0, total_time, num_samples, endpoint=False)

#Generate sine wave
signal = np.sin(2 * np.pi * f_signal * t)

#Plotting
plt.figure(figsize=(10, 6))
plt.plot(t * 1e9, signal)  #, marker='o')
plt.title('2 MHz Sine Wave')
plt.xlabel('Time (ns)')
plt.ylabel('Amplitude')
plt.grid(True)
plt.show()

plt.tight_layout()
plt.show()
plt.savefig("lab-fsk.png")
```

### Modulation
```py
#!/usr/bin/env python3

import numpy as np
import matplotlib.pyplot as plt
from scipy.fft import fft, fftfreq
## For saving plots to a file. Just couldn't get it to work from commandline
import matplotlib
matplotlib.use('Agg')

# Parameters
fc0 = 4e6        # 1 Carrier Frequency
fc1 = 2e6        # 0 Carrier Frequency
fs = 256*4e6    # Sampling frequency
ncycl = 512          # No of cycles of fc 
nfc0 = 8        # number of fc0 cycles for one symbol
Tsim = ncycl/fc0       # Total Simulation time
t = np.arange(0, Tsim, 1/fs)  # Time vector

# Message signal (binary data)
data = np.random.randint(0, 2, int(ncycl/nfc0))  # Random binary data
nupData = int(t.size/data.size) 
data = np.repeat(data, nupData)  # Upsample binary data

# FSK Modulation
modulated_signal = np.zeros_like(t)
for i in range(len(t)):
    if data[i] == 0:
        modulated_signal[i] = np.cos(2 * np.pi * fc0 * t[i])
    else:
        modulated_signal[i] = np.cos(2 * np.pi * fc1 * t[i])

# FFT of the modulated signal
N = len(modulated_signal)
yf = fft(modulated_signal)
xf = fftfreq(N, 1 / fs)

# modulation
# Parameters for modulation
threshold = 0  # Decision threshold for modulation

# modulated data array
modulated_data = np.zeros_like(data)

# modulation loop
for i in range(len(t)):
    if np.cos(2 * np.pi * fc0 * t[i]) > threshold:
        modulated_data[i] = 0
    else:
        modulated_data[i] = 1

# Ensure demodulated data has the correct length (may be longer due to upsampling)
modulated_data = modulated_data[:data.size]

# Plotting
fig, axs = plt.subplots(4, 1, figsize=(10, 16))

axs[0].plot(t, data)
axs[0].set_title('Original Binary Data')
axs[0].set_xlim([0, Tsim])
axs[0].set_ylim([-0.2, 1.2])

axs[1].plot(t, modulated_signal)
axs[1].set_title('FSK Modulated Signal')
axs[1].set_xlim([0, Tsim])

axs[2].plot(xf, np.abs(yf))
axs[2].set_title('FFT of Modulated Signal')
axs[2].set_xlim([0, 2*fc0])
axs[2].set_xlabel('Frequency (Hz)')

axs[3].plot(t, modulated_data, marker='o', linestyle='-', color='b')
axs[3].set_title('modulated Binary Data')
axs[3].set_xlabel('Time (s)')
axs[3].set_ylabel('Binary Value')
axs[3].set_xlim([0, Tsim])
axs[3].set_ylim([-0.2, 1.2])
axs[3].grid(True)

plt.tight_layout()
plt.savefig("fsk-lab2.png")
plt.show()
```
![demodulation](https://github.com/user-attachments/assets/f42470f5-bce1-44cc-8887-c178199f7a58)

## Demodulation
```py

# Parameters
fc0 = 4e6        # 1 Carrier Frequency
fc1 = 2e6        # 0 Carrier Frequency
fs = 256*4e6    # Sampling frequency
ncycl = 512          # No of cycles of fc
nfc0 = 8        # number of fc0 cycles for one symbol
Tsim = ncycl/fc0       # Total Simulation time
t = np.arange(0, Tsim, 1/fs)  # Time vector

# Message signal (binary data)
data = np.random.randint(0, 2, int(ncycl/nfc0))  # Random binary data
nupData = int(t.size/data.size)
data = np.repeat(data, nupData)  # Upsample binary data

print(data.size, t.size)

# FSK Modulation
modulated_signal = np.zeros_like(t)
for i in range(len(t)):
    if data[i] == 0:
        modulated_signal[i] = np.cos(2 * np.pi * fc0 * t[i])*np.cos(2 * np.pi * fc0 * t[i])
    else:
        modulated_signal[i] = np.cos(2 * np.pi * fc1 * t[i])*np.cos(2 * np.pi * fc0 * t[i])

# FFT of the modulated signal
N = len(modulated_signal)
yf = fft(modulated_signal)
xf = fftfreq(N, 1 / fs)

# Plotting
fig, axs = plt.subplots(3, 1, figsize=(10, 12))

axs[0].plot(t, data)
axs[0].set_title('Original Binary Data')
axs[0].set_xlim([0, Tsim])
#axs[0].set_ylim([-0.2, 1.2])

axs[1].plot(t, modulated_signal)
axs[1].set_title('FSK DeModulation')
axs[1].set_xlim([0, Tsim])
                                                                                                                                                        axs[2].plot(xf, np.abs(yf))
axs[2].set_title('FFT of DeModulated Signal')
axs[2].set_xlim([0, 2*fc0])
axs[2].set_xlabel('Frequency (Hz)')

plt.tight_layout()
plt.savefig("fsk-demodulation-lab2.png")
plt.show()
```

![fsk-demodulation-lab2](https://github.com/user-attachments/assets/7835a516-0691-4310-8959-ea1308133588)




## Lab 9: I2C temperature sensor interface

![cf5729a0-1bd2-4b48-b892-6fc4948ee1ed](https://github.com/user-attachments/assets/65251995-6613-4899-8ec7-0e96cfb8c69b)

```c
#include<Wire.h>
#include<Adafruit_GFX.h>
#include<Adafruit_SSD1306.h>
#include<Adafruit_Sensor.h>
#include "DHT.h"

#define SCREEN_WIDTH 128 //128OLED DISPLAY WIDTH
#define SCREEN_HEIGHT 64

Adafruit_SSD1306 display(SCREEN_WIDTH,SCREEN_HEIGHT,&Wire,-1);

#define DHT11PIN 4

#define DHTTYPE DHT11
DHT dht(DHT11PIN, DHTTYPE);

void setup(){
  Serial.begin(9600);
  dht.begin();

  if(!display.begin(SSD1306_SWITCHCAPVCC,0X3C)){
    Serial.println(F("SSD1306 allocation failed"));
    for(;;);
  }
  delay(2000);
  display.clearDisplay();
  display.setTextColor(WHITE);
}

void loop(){
  delay(5000);

  float humi = dht.readHumidity();
  float temp = dht.readTemperature();
  if(isnan(humi)||isnan(temp)){
    Serial.println("Failed to read from DHT sensor!");
  }

  display.clearDisplay();

display.setTextSize(1);
display.setTextColor(SSD1306_BLACK,SSD1306_WHITE);
display.setCursor(0,0);
display.print("temperature");
display.setTextSize(2);
display.setTextColor(SSD1306_BLACK,SSD1306_WHITE);
display.setCursor(0,10);
display.print(temp);
display.print(" ");
display.setTextSize(2);
display.print("C");


display.setTextSize(1);
display.setTextColor(SSD1306_BLACK,SSD1306_WHITE);
display.setCursor(0,35);
display.print("HUMIDITY");
display.setTextSize(2);
display.setTextColor(SSD1306_BLACK,SSD1306_WHITE);
display.setCursor(0,45);
display.print(humi);
display.print(" %");

display.display();
}
```





## Lab 10: Introduction to LoRa module

Introduction to architecture and pin configuration of Ra-02 Lora transceiver module and SPI (Serial Peripheral Interface) communication.

Key Features
-Long Range: Achievable distances from several kilometers up to 15 km or more.
-Low Power: Suitable for battery-operated devices, often using deep sleep modes.
-Low Data Rate: Typically supports data rates from 0.3 kbps to 50 kbps, which is sufficient for many IoT applications.

**Connect the LoRa module to your ESP32 (e.g., using SPI pins).**

|Module Pin	|Arduino Pin|
|-----------|-----------|
|VCC|3.3V|
|GND|GND|
|SCK|Pin 13|
|MOSI|Pin 11|
|MISO|Pin 12|
|NSS|Pin 10|
|RESET|Pin 9|
|DIO0|Pin 2|

**Ra-02 (SX1278)**

Frequency: 433/868/915 MHz
Range: Up to 15 km in rural areas
Interface: SPI
Commonly used with Arduino and ESP32.





## Lab 12: Communication between two LoRa nodes

Sending Text packets and receiving the text packets with *RSSI (Received Signal
Strength Indicator)* and SNR through Serial monitor.
Sending Temperature and humidity packets and receiving the same packets with RSSI (Received Signal Strength Indicator) and SNR through a Serial monitor as well as an OLED display.

### Programming for Transmitter Station

```c
#include<SPI.h>
#include<LoRa.h>

//std configuration
//#define DIO0 2
//#define RST 14
//#define NSS 3
//#define MOSI 23
//#define MISO 19
//#define SCLK 18

#define DIO0 26
#define RST 14
#define NSS 18
#define MOSI 27
#define MISO 19
#define SCLK 5

int counter=0;

void setup(){
  //initiliazing serial monitor
  Serial.begin(115200);
  while(!Serial);
  Serial.println("LoRa Sender");

  //setup LoRa tranceiver module
  SPI.begin(SCLK,MISO,MOSI,NSS);
  LoRa.setPins(NSS,RST,DIO0);

  //replace the lora.begin(---E-)
  // 433E6 FOR ASIA
  // 866E6 FOR EUROPE
  // 915E6 FOR NORTH AMERICA
while(!LoRa.begin(433E6)){
  Serial.println(".");
  delay(500);
}
//change sync word 0xF3 to match reciever
//the sync word assures you dont gets LoRa message from other LoRa transceiver
//ranges from 0-0xFF
LoRa.setSyncWord(0XF3);
Serial.println("LoRa Initializing OK !");
}

void loop(){
  Serial.println("sending packet");
  Serial.println(counter);

  //send LoRa packet to recieve

  LoRa.beginPacket();
  LoRa.print("hello...");
  LoRa.print(counter);
  LoRa.endPacket();

  counter++;

  delay(1000);
}

```
### Programming for Reciever Station
```c
#include<SPI.h>
#include<LoRa.h>

//std configuration
//#define DIO0 2
//#define RST 14
//#define NSS 3
//#define MOSI 23
//#define MISO 19
//#define SCLK 18

#define DIO0 26
#define RST 14
#define NSS 18
#define MOSI 27
#define MISO 19
#define SCLK 5


void setup(){
  //initiliazing serial monitor
  Serial.begin(115200);
  while(!Serial);
  Serial.println("LoRa Sender");

  //setup LoRa tranceiver module
  SPI.begin(SCLK,MISO,MOSI,NSS);
  LoRa.setPins(NSS,RST,DIO0);

  //replace the lora.begin(---E-)
  // 433E6 FOR ASIA
  // 866E6 FOR EUROPE
  // 915E6 FOR NORTH AMERICA
while(!LoRa.begin(433E6)){
  Serial.println(".");
  delay(5000);
}
//change sync word 0xF3 to match reciever
//the sync word assures you dont gets LoRa message from other LoRa transceiver
//ranges from 0-0xFF
LoRa.setSyncWord(0XF3);
Serial.println("LoRa Initializing OK !");
}

void loop() {
  // try to parse packet
  int packetsize = LoRa.parsePacket();
  if(packetsize){
    Serial.println("Recieving Packet:");
  }
  while(LoRa.available()){
    String LoRaData = LoRa.readString();
    Serial.print(LoRaData);
  }
    Serial.print("`with RSSI");
    // RSSI - recieved signal strength indicator
    Serial.print(LoRa.packetRssi());
    Serial.println("C");
  }
```
|Sl No.|Transmission Power|RSSI|🔺RSSI|
|------|------------------|----|-------|
|1|0|62.3|0|
|2|1|5|51.4|10.9|
|3|7|50.6|11.7|

## Lab 13: LoRa one-to-many communication setup

Sending data packets from one Lora transmitter to multiple Lora receivers and retracing the same packets.

![d2727fe6-5d07-46f3-9c0b-39a2f445ded9](https://github.com/user-attachments/assets/50f08491-6c53-44ea-8836-33d0de2a9624)


### Programming for transmission

```c
#include<SPI.h>
#include<LoRa.h>

//std configuration
//#define DIO0 2
//#define RST 14
//#define NSS 3
//#define MOSI 23
//#define MISO 19
//#define SCLK 18

#define DIO0 26
#define RST 14
#define NSS 18
#define MOSI 27
#define MISO 19
#define SCLK 5

int counter=0;

void setup(){
  //initiliazing serial monitor
  Serial.begin(115200);
  while(!Serial);
  Serial.println("LoRa Sender");

  //setup LoRa tranceiver module
  SPI.begin(SCLK,MISO,MOSI,NSS);
  LoRa.setPins(NSS,RST,DIO0);

  //replace the lora.begin(---E-)
  // 433E6 FOR ASIA
  // 866E6 FOR EUROPE
  // 915E6 FOR NORTH AMERICA
while(!LoRa.begin(433E6)){
  Serial.println(".");
  delay(500);
}
//change sync word 0xF3 to match reciever
//the sync word assures you dont gets LoRa message from other LoRa transceiver
//ranges from 0-0xFF
LoRa.setSyncWord(0XF3);
Serial.println("LoRa Initializing OK !");
}

void loop(){
  Serial.println("sending packet");
  Serial.println(counter);

  //send LoRa packet to recieve

  LoRa.beginPacket();
  LoRa.print("hello...");
  LoRa.print(counter);
  LoRa.endPacket();

  counter++;

  delay(1000);
}

```
### Programming for reciever
```c
#include<SPI.h>
#include<LoRa.h>

//std configuration
//#define DIO0 2
//#define RST 14
//#define NSS 3
//#define MOSI 23
//#define MISO 19
//#define SCLK 18

#define DIO0 26
#define RST 14
#define NSS 18
#define MOSI 27
#define MISO 19
#define SCLK 5


void setup(){
  //initiliazing serial monitor
  Serial.begin(115200);
  while(!Serial);
  Serial.println("LoRa Sender");

  //setup LoRa tranceiver module
  SPI.begin(SCLK,MISO,MOSI,NSS);
  LoRa.setPins(NSS,RST,DIO0);

  //replace the lora.begin(---E-)
  // 433E6 FOR ASIA
  // 866E6 FOR EUROPE
  // 915E6 FOR NORTH AMERICA
while(!LoRa.begin(433E6)){
  Serial.println(".");
  delay(5000);
}
//change sync word 0xF3 to match reciever
//the sync word assures you dont gets LoRa message from other LoRa transceiver
//ranges from 0-0xFF
LoRa.setSyncWord(0XF3);
Serial.println("LoRa Initializing OK !");
}

void loop() {
  // try to parse packet
  int packetsize = LoRa.parsePacket();
  if(packetsize){
    Serial.println("Recieving Packet:");
  }
  while(LoRa.available()){
    String LoRaData = LoRa.readString();
    Serial.print(LoRaData);
  }
    Serial.print("`with RSSI");
    // RSSI - recieved signal strength indicator
    Serial.print(LoRa.packetRssi());
    Serial.println("C");
  }
```






## Lab 14: Introduction to antenna modeling and simulation software 4NEC2.

**4NEC2** is a popular antenna modeling and simulation tool based on the Numerical Electromagnetics Code (NEC). It allows users to design, analyze, and optimize antennas by simulating their performance in various configurations.

### Key Features
  -  **Easy to Use:** User-friendly interface suitable for beginners and experienced users alike.

  -  **Versatile Modeling:** Supports various antenna types, including dipoles, Yagi-Uda, and more complex designs.

  -  **Visual Representation:** Provides graphical visualization of antenna geometry and radiation patterns.

  -  **Post-Processing:** Allows for in-depth analysis of results, including gain, radiation patterns, and impedance.






## Lab 15: Physical design of Dipole and V-dipole antennas

Tune it to 433MHz with the help of NanoVNA-A Portable VNA Antenna Analyzer Kit with 10KHz-1.5GHz, 2.8 Inch Digital LCD Display Touching Screen Standing Wave Measuring Instrument.

```txt
CM Example new :	Loaded dipole in free space
CM 		antenna design.txt
CE 					' End of comment
'


SY ylen=.1392				' Symbol: Length for WL/2
SY zlen=.0975
SY ysma=.004095
SY zsma=.002867	
'

GW  1  9  0  -ylen   zlen   0  -ysma  zsma   .0001	' Wire 1, 9 segments, halve wavelength long.
GW  2  9  0   ysma   zsma   0   ylen  zlen   .0001	' Wire 2, 9 segments, halve wavelength long.
GW  3  1  0  -ysma   zsma   0   ysma  zsma   .0001	' Wire 3, 9 segments, halve wavelength long
GE  0					' End of geometry
'


LD 5 1 0 0 5.8001E7			' Wire conductivity
LD 5 2 0 0 5.8001E7			
LD 5 3 0 0 5.8001E7			


'


EX 0 3 1 0 1 0				' Voltage source (1+j0) at wire 1 segment 5.


FR 0 1 0 0 433 0			' Set design frequency (433 Mc).

EN					' End of NEC input

```
![image](https://github.com/user-attachments/assets/bf7da8ba-95b8-4a00-b354-6a23631f242a)

![image](https://github.com/user-attachments/assets/5b4f47b9-ff8a-4d6e-a8b4-667a1a91bc43)

**Lab 16: Introduction to TinyGS**

**Lab 17: Setting up a TinyGS ground station**



# Setting up TinyGS groundstation

![Screenshot (499)](https://github.com/user-attachments/assets/bce919be-5187-4200-958e-4db33bdee0ae)






## Lab 18: Processing TLE data with Python

**Using genAI tool (ChatGPT, CoPilot, etc) find out the detail about the satellite Two-Line Element (TLE) format.**

https://api.tinygs.com/v1/tinygs_supported.txt

**Write a Python programm to conver a TLE of satellite into a Lat/Long location.**

```py
rom skyfield.api import EarthSatellite, load
from datetime import datetime
import time
import webbrowser

def generate_maps_url(latitude, longitude):
    return f"https://www.google.com/maps/search/?api=1&query={latitude},{longitude}"

def main():
    try:
        # Prompt user to input TLE data
        print("Enter TLE data:")
        line1 = input("Enter line 1: ").strip()
        line2 = input("Enter line 2: ").strip()

        # Extract satellite name from line 1 if available
        satellite_name = line1.split()[1]

        # Load TLE data into a satellite object
        satellite = EarthSatellite(line1, line2, name=satellite_name)

        # Load timescale
        ts = load.timescale()

        while True:
            # Get current UTC time
            now = datetime.utcnow()

            # Compute satellite position at the current time
            t = ts.utc(now.year, now.month, now.day, now.hour, now.minute, now.second + now.microsecond / 1e6)
            position = satellite.at(t)

            # Get GeographicPosition object
            geo_position = position.subpoint()

            # Extract latitude, longitude, and altitude in degrees and kilometers
            latitude = geo_position.latitude.degrees
            longitude = geo_position.longitude.degrees

            print(f" ")
            print(f"{satellite_name}")
            print(f"Latitude, Longitude: {latitude}, {longitude}")

            # Calculate altitude (height above Earth's surface)
            distance_from_earth_center = position.distance().km
            radius_of_earth = 6371.0  # Radius of the Earth in kilometers
            altitude = distance_from_earth_center - radius_of_earth

            print(f"Altitude: {altitude} km")

            # Generate Google Maps URL
            maps_url = generate_maps_url(latitude, longitude)
            print(f"Google Maps URL: {maps_url}")

            # Open Google Maps in the default web browser
            webbrowser.open(maps_url)

            # Delay for a while before fetching the next position
            time.sleep(10)  # Fetch position every 10 seconds (adjust as needed)

    except KeyboardInterrupt:
        print("\nTerminated by user.")
    except Exception as e:
        print(f"Error occurred: {e}")

if _name_ == "_main_":
    main()
```


**Enter TLE data: TIANQI-23**

    Enter line 1: 1 57794U 23135C   24193.84851663  .00000031  00000-0  84750-4 0  9998

    Enter line 2: 2 57794  49.9717 238.8296 0014532 317.7298  42.2493 14.22337202 44201

**Generate the output as an URL that you can paste in a browser and get the satellite location.**

https://www.google.com/maps/place/25%C2%B024'17.5%22N+30%C2%B015'50.8%22W/@25.4048723,-30.2641009,17z/data=!3m1!4b1!4m4!3m3!8m2!3d25.4048723!4d-30.2641009?entry=ttu

![image](https://github.com/user-attachments/assets/ef600973-5b49-40b0-8bfb-035cf8087903)


And modify the above program such the TLE data file can be given as input with the two line numbers to process.

