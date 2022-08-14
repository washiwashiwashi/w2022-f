Engineering materials
====
This repository contains engineering materials of a self-driven vehicle's model participating in the WRO Future Engineers competition in the season 2022.

## Introduction
Our team is "Otemon Curiocity". There are two people in our team.
* country-Japan
* Akimitsu Fujimura/Programmer robot designer
* Masamu Yasui/Programmer 

## About the Robot
* This self-driving car is mainly made by LEGO, and parts that are not available in LEGO are created using a 3D printer.

## The hardware
| what to use | Details |
|:---|:---:|
| LEGO spike prime | To run automatic cars |
| BBC microbit | To process image recognition |
| Huskylens | To recognize traffic signals |
| RGB LED | To communicate between microbit and spike |
| LED | To increase the recognition rate of huskylens traffic signals |
| L motor | Rear wheel motors |
| M motor | To be used in steering |
| color sensor | The front color sensor is used to read the color of the coat (blue and orange lines), and the two color sensors in the middle are used to read the rgb led information (blue, green, and red) output from the microbit and send commands to the legto spike prime.Therefore,the color sensor would be one of the very important sensors. |
| ultrasonic sensor | Ultrasonic sensors are used to detect and deflect objects. It is located in front of the robot｜

## The software
Since this robot uses spike and microbit, the language is a visual language. spike uses the LEGO® Education SPIKE™ app, MakeCode for micro:bit, and downloads the program.The programs is in `src`.

## The good thing about this robot
1.The robot has a simple structure and the system is not that complicated,
The system is not that complicated, and it is not difficult to deal with any problems.

2.When a part breaks down, it can be fixed with LEGO, rather than having to go to the trouble of remaking the main part with a 3D printer.

3.The robot shall be able to raise the accuracy of signal recognition without misrecognizing traffic signals and the blue and orange lines by installing two leds on the front of the robot.

4.That the use of lego spike prime will allow it to move smoothly, probably because of the color sensor and the motor's increased performance.

5.In addition, waste was reduced by making some parts with a 3D printer. The reason why only some parts were made with a 3D printer is because there are some parts that cannot be made with lego parts alone, and it is impossible to make them with lego parts alone. Also, to make it easier for the color sensor to read the led, a special container was made, which made it easier to read the led.

6.As you can see in the photo from the bottom of the `v-photo`, it uses differential gears on the rear wheels, and the differential gears are responsible for transmitting the power from the engine to both the left and right wheels, while absorbing the difference in speed between the inside and outside of the curve, so that the car turns smoothly!

7.Why we chose the huskylens camera--we first tried to use raspberry pi to recognize traffic signals using opencv, but we had trouble with the cascade turnouts and were frustrated, then we considered m5stickC, etc., but after considering system We considered using a microbit to run huskylens, considering compatibility, etc., and did. huskylens is accurate, performs well, and is less convenient, although power is only slightly different.

8.The battery is loaded with rechargeable batteries and can be recharged efficiently.

9.The structure from the differential gear to the tire is good, and if the shaft is used as it is, there is a risk that the shaft will be overloaded and break, or that the car will not run smoothly.

10.Strong fixation of tires. A shaft shaped like a nail was used to make it difficult to pull out.
 
11.We used lego spike prime and microbit because the lego spike prime has a good motor that does not easily shift the rotation speed or angle (if it does, it is less than 3 degrees), and the color sensor also has good performance, with high accuracy in color discrimination and thresholds.

## What is wrong with this robot
1.What huskylens does with color recognition, not object recognition. The reason for this is that when there is a person or object outside the coat, color recognition, as the name implies, recognizes only the color, so the probability of misrecognition is higher. The reason it is not object recognition is that huskylens is not very good when it comes to object recognition.

2.That there is a delay because the microbit and lego spike prime are not directly connected, but the color sensor is reading the color depending on the color of the led and whether it is physically lit. This can't be helped, but in the future, after the competition, we will research if it is possible to connect directly between lego spike prime and microbit, or instead of using lego spike prime itself as a computer, we will use raspberrypi4B for image recognition and arduino for driving. We are thinking of using raspberrypi4B for image recognition and arduino for driving.

## Thoughts on future engineers competitions after
* Try various single board computers and other equipment without using LEGO products, and try the next competition.
* Learn image recognition using opencv, etc.
* Create a self-driving car with machine learning, using tensorflow.
