# **Ultrasonic Proximity Detection System Using Arduino UNO**

## **1\. Aim**

To develop an Arduino-based proximity detection system that measures the distance of an object using an **HC-SR04 ultrasonic sensor** and provides a visual indication through an **LED** when the object approaches a predefined distance.

## **2\. Components Required**

1. Arduino UNO  
2. HC-SR04 Ultrasonic Sensor  
3. LED  
4. 220Ω Resistor  
5. Breadboard  
6. Male-to-Male Jumper Wires  
7. USB Cable  
8. Computer/Laptop for programming

## **3\. Introduction**

Distance measurement is an important function in many automation and embedded systems. In this project, an **HC-SR04 ultrasonic sensor** is interfaced with an **Arduino UNO** to detect the distance between the sensor and a nearby object.

The measured distance is processed by the Arduino, and an LED is activated when the object enters the predefined detection range. This provides a simple and effective method of demonstrating **object proximity detection**.

## **4\. Working Principle**

The HC-SR04 operates based on the **ultrasonic echo principle**. The sensor consists of a transmitter and receiver.

The transmitter emits an ultrasonic pulse at approximately **40 kHz**. When the sound wave encounters an object, it is reflected back toward the sensor. The receiver detects the returning echo, and Arduino determines the distance by measuring the time taken for the echo to return.

The distance is calculated using:

**Distance \= (Time × Speed of Sound) / 2**

The division by 2 is required because the ultrasonic wave travels from the sensor to the object and then back to the sensor.

## **5\. Methodology / Working Procedure**

1. The HC-SR04 sensor is connected to the Arduino UNO.  
2. The Arduino sends a short trigger pulse to the ultrasonic sensor.  
3. The sensor transmits an ultrasonic sound wave toward the object.  
4. The wave is reflected when it encounters the object.  
5. The sensor receives the reflected echo.  
6. Arduino measures the echo duration and calculates the corresponding distance.  
7. The measured distance is compared with a predefined threshold value.  
8. If the object is within the specified range, the LED is switched ON.  
9. If the object moves beyond the specified range, the LED remains OFF.

## **6\. Circuit Description**

The **VCC** and **GND** pins of the HC-SR04 are connected to the corresponding power and ground pins of the Arduino UNO. The **TRIG** and **ECHO** pins are connected to Arduino digital pins for transmitting and receiving the ultrasonic signal.

An LED is connected to another digital output pin through a **current-limiting resistor**. The Arduino controls the LED based on the distance detected by the ultrasonic sensor.

**Suggested circuit connections:**

| Component | Arduino UNO |
| ----- | ----- |
| HC-SR04 VCC | 5V |
| HC-SR04 GND | GND |
| HC-SR04 TRIG | Digital Pin 9 |
| HC-SR04 ECHO | Digital Pin 10 |
| LED Anode (+) | Digital Pin 13 through resistor |
| LED Cathode (-) | GND |

## **7\. Advantages**

* Simple and low-cost implementation  
* Contactless distance measurement  
* Easy to program and modify  
* Suitable for beginners in embedded systems  
* Provides real-time object detection  
* Can be extended with additional sensors or indicators

## **8\. Applications**

The system can be used in:

* Obstacle detection systems  
* Parking assistance systems  
* Automatic door mechanisms  
* Smart waste bins  
* Robotic navigation  
* Proximity warning systems  
* Industrial object detection  
* Basic security and automation systems

## **9\. Result**

The **Arduino-based ultrasonic proximity detection system** was successfully designed and implemented. The HC-SR04 sensor accurately detects the presence of an object by measuring its distance, while the LED provides a visual indication when the object enters the defined detection range.

## **10\. Conclusion**

This project demonstrates the practical application of **ultrasonic sensing and Arduino-based control**. It provides a basic understanding of distance measurement, sensor interfacing, digital output control, and embedded-system programming. The developed system can serve as a foundation for more advanced automation and obstacle-detection applications.

