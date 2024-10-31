<h1 align="center" style="font-size:20">
Introduction to Robotics Course
</h1>

<p align="center">
Everything related to the course.
</p>

<p align="center">
  :microscope: <a href="#about">About</a>&#160;
  :pencil: <a href="#content">Content</a>&#160;
</p>

## About

#### Course Objectives:
1. Development of POC (Proof of Concept) and Final Product Development Skills
2. Encouragement of Critical Thinking and Problem Solving
3. Programming Skills Development
4. Understanding Basic Robotics Concepts
5. Understanding and Using Microcontrollers

Professor: [Dan Tudose](https://github.com/dantudose)

Laboratory tutor: [Radu Ioan Nedelcu](https://github.com/Pepi100)

</br>

## Content

### PROJECT 1: Electric vehicle charging system
<details>
<summary>TASK</summary> 
 
  
<img src="media/project 1/img/Screenshot 2024-10-23 210012.png" align="right" alt="Diagram" width="400">



#### Components Used

- 4x LEDs (to simulate the percentage of charge)
- 1x RGB LED (for free or busy status)
- 2x Buttons (for charging start and stop charging)
- 8x Resistors (6x 220/330ohm, 2x 1K)
- Breadboard
- Connecting Lines

</br>
</br>
</br>

#### Technical Task

The RGB LED represents the availability of the station. If the station is free, the LED will be green, and if the station is occupied, it will turn red.
The simple LEDs represent the degree of battery charge, which we will simulate through a progressive loader (L1 = 25%, L2 = 50%, L3 = 75%, L4 = 100%). The loader is charged by successively lighting up the LEDs, at a fixed interval of 3s. The LED that signifies the current percentage of charge will have a flashing state, the LEDs behind it being lit continuously, and the others turned off.
Short pressing the start button will start charging. Pressing this button while charging will not do anything.
Long pressing the stop button will forcibly stop charging and reset the station to the free state. Pressing this button while the station is free will not do anything.

</br>
</br>
</br>

</details>

<details>
<summary>IMPLEMENTATION</summary> 

</br>

[Virtual Simulation](https://wokwi.com/projects/412558654532609025)
</br>

[Code](https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/code/project%201/main.cpp)
</br>

[Video of the physical setup](https://imgur.com/VyJZZNH)
</br>

#### Photo Gallery

<div align="center">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(1).jpg" alt="Image 1" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(2).jpg" alt="Image 2" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(3).jpg" alt="Image 3" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(4).jpg" alt="Image 4" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(5).jpg" alt="Image 5" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(6).jpg" alt="Image 6" width="300">  
</div>

</br>
</br>
</details>



### PROJECT 2: ⁠TypeRacer Game
<details>
<summary>TASK</summary> 
 
  
<img src="media/project 1/img/Screenshot 2024-10-23 210012.png" align="right" alt="Diagram" width="400">

#### Description

In this theme you will create a game similar to TypeRacer.

</br>

#### Components Used

- Arduino UNO (ATmega328P microcontroller)
- 1x RGB LED (to signal if the correct word is misspelled or not)
- 2x Buttons (for round start/stop and difficulty selection)
- 5x Resistors (3x 220/330 ohm, 2x 1000 ohm)
- Breadboard
- Connecting threads

</br>

#### Technical Task

RGB LED - Status indicator:

In the sleep state, the LED will be white.
When the start button is pressed, the LED will flash for 3 seconds, indicating a countdown until the start of the round.
During a round: The LED will be green if the text entered is correct and will turn red if there is an error.
(1p) Start/Stop button:

Sleep Mode: If the game is paused, pressing the button initiates a new round after a 3-second countdown.
During a round: If the round is active, pressing the button will stop it immediately.
(1p) Difficulty button:

The difficulty button controls the speed at which words appear and can only be used in idle mode.
With each press, the difficulty changes by cycling between: (Easy, Medium, Hard).
When changing the difficulty, a message is sent via serial: "Easy/Medium/Hard mode on!".
For handling button presses, use debouncing and interrupts. Timers will be used to set the frequency of occurrence of words. A useful site, which also includes a video on using interrupts and timers in Arduino, is available here.
(3p) Word generation:

A word dictionary will be created.
During a round, the words will be displayed in the terminal in a random order.
If the current word was spelled correctly, a new word will be displayed immediately. If not, a new word will appear after the time interval set by the difficulty.
To generate random numbers, you must use the random() function.
(1p) Other observations:

The allotted time for a round is 30 seconds.
At the end of each round, the terminal will display how many words were spelled correctly.
</br>
</br>
</br>

</details>

<details>
<summary>IMPLEMENTATION</summary> 

</br>

[Virtual Simulation](https://wokwi.com/projects/413099200289435649)
</br>

[Code](https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/code/project%201/main.cpp)
</br>

[Video of the physical setup](https://imgur.com/VyJZZNH)
</br>





#### Photo Gallery

<div align="center">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(1).jpg" alt="Image 1" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(2).jpg" alt="Image 2" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(3).jpg" alt="Image 3" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(4).jpg" alt="Image 4" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(5).jpg" alt="Image 5" width="300">
  <img src="https://github.com/calinfrunzeanu/Introduction-to-Robotics/blob/main/media/project%201/img/tema%201%20img%20(6).jpg" alt="Image 6" width="300">  
</div>

</br>
</br>
</details>
