# DIY-Stick-Catching-Game
It's a game machine that tests your reflexes.


#throwback-may-2023

![image alt](https://github.com/Anandhu-Sudha/DIY-Stick-Catching-Game/blob/e082bec50591835b414cc214d53c8455862b65d3/pictures/Screenshot%202025-02-01%20225637.png)

During the time of college techno-cultural festival I've made a small game machine, Not sure about it's name but let's call it  " Stick Catching Game ". I've seen this in many videos that are placed in festival areas. I wanted to make one of those and when the time has come, I've decided to make one with the help of my friends.

Sadly there's no proper documentation for this also. It was back in the day i used to make stuff like this for my own joy and never had a thought about documenting it one day.

<b>Construction</b>
------------------

The process was simple, Attached 8 micro servos to an aluminium frame equally spaced apart. A hook shaped piece made of a material called 'Forex' ( light and pretty rigid). All servos vcc & gnd are wired together and connected the 8 signal pins to 8 different GPIO pins in an Arduino UNO. 

![image alt](https://github.com/Anandhu-Sudha/DIY-Stick-Catching-Game/blob/e082bec50591835b414cc214d53c8455862b65d3/pictures/WhatsApp%20Image%202025-02-01%20at%2023.03.33_d1a00daf.jpg)

Me and my boys fixing things at the last moment (like always 😁 ).

![image alt](https://github.com/Anandhu-Sudha/DIY-Stick-Catching-Game/blob/fd602a7df13a1b1446394a8c52a9e085b30b0ce2/pictures/WhatsApp%20Image%202025-01-28%20at%2022.30.44_dab69a05.jpg)


<b>Coding</b>
-------------
With the help of 'random()' - It generates random numbers, by using randomly generated numbers between 1 & 8 using if condition each servos are controlled randomly.
When the if() becomes true for servos, the servo rotates an angle enough to slip the stick attached to the hook at the end of these servos.
Also by adjusting delay the difficulty of game can also be increased.

By adding a physical toggle switch to the game, it can decide the difficulty level of the game. 1. Easy mode 2. Hard Mode.
When the switch is in off position a set of instruction works for the easy section with larger delays where as when the switch is on another set of instruction works for the Harder section where the delays are small and the sticks falls quickly one after another.

Although the rig was a success and attracted a lot of attention there was some room for improvement.
1. The servo was struggling to hold the stick after continuous usage, I was using sg90 servos ( basic blue servos) their torque capacity is only 1.3kg/cm. So either lightweight sticks or servos with better torque was needed.
2. The Stand made using aluminium had some flaws, it was obstructing the players hands. some people's hands left imprints on the frame after intensely focusing on game 😂. The stand was also made in such a way that it should be stable , but somehow due to lack of time, that was not fixed.

Apart from these minor issues, I consider this as a great success considering it's made within a day.

Some Clips of the Gameplay is attached below.

Easy Mode 👇

https://github.com/user-attachments/assets/1d348d8f-f934-4de7-a801-8d6c6fc457e4

Hard Mode 👇

https://github.com/user-attachments/assets/7ef7f93a-fe91-4a4a-9296-c846ae94926f


