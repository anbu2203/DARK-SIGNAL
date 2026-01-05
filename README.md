 ## Dark Signal: The Batman Blinky Board
Building this project was a huge milestone for me. I wanted to move beyond a basic "LED on a breadboard" and create something that actually looked like it belonged in Gotham. Using the Hack Club guide was a game-changer; it turned the intimidating world of PCB design into a fun, step-by-step puzzle that I actually enjoyed solving.
## PCB IMAGES
![3D PCB FRONT](README%20IMAGES/3D%20PCB%20FRONT.png)
It showcases the 3mm Red LEDs following the curves of the wings and the NE555P/4017 chips acting as the central "engine."
The Potentiometer (RV1) is prominently placed, allowing the user to manually dial in the speed of the chasing lights.
![3D PCB BACK](README%20IMAGES/3D%20PCB%20BACK.png)
This view highlights the clean copper paths that carry signals between the chips and the LEDs. It shows the tidy Through-Hole pads where the components will be permanently joined to the board, giving it a professional, high-quality finish.
![PCB EDITOR](README%20IMAGES/PCB%20EDITOR.png)
The board outline is a custom DXF import on the Edge.Cuts layer, creating the bat-wing shape. This view shows the "rat's nest" turned into organized traces on both the Top (Red) and Bottom (Blue) copper layers to avoid collisions.The LEDs are balanced across both wings to ensure the light sequence looks uniform when the board is powered on.
## schematic 
![SCHEMATIC](README%20IMAGES/SCHEMATIC.png)
The NE555P is wired in Astable Mode, creating a continuous pulse that acts as the heartbeat for the lights. You can see Pin 3 (OUT) of the 555 timer feeding directly into Pin 14 (CLK) of the 4017 counter to drive the animation.A 470 Ω resistor (R1) is placed at the end of the LED chain to limit current and prevent the LEDs from burning out.
## thanks
Huge thanks to the Hack Club community for the guidance and inspiration. This project turned a bunch of random components into a pulsing Bat-signal, and I couldn't be more proud of the final "ship."
## bill of materials (BOM)
-1uF capacitor x 1
-0.01uF capacitor x 1
-led x 10
-1k resistor x 1
-470 ohm resistor x 1
-50K resistor x 1
-testpoint connector x 3
-NEE555P IC x 1
-4017 IC x 1
-tOTAL Estimated Build Cost=$15.15 - $20.15
