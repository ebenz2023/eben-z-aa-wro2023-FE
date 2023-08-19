
FUTURES ENGINEERING
SENIOR

TEAM: EBEN-Z-AA

Integrants: 
•	Aguilar, Amira
•	Burke, Paulette
•	Martínez-Aparicio, Álvaro 

Affair: Report













Introduction
Our robot (Indie) is an autonomous automotive vehicle powered by three motors, two for propulsion and one for steering. It is equipped with sensors that guide the vehicle through predefined obstacles. All of this functionality is enabled by the Hub (brain) and Spike's programming.

Design Process:
Mechanics
•	Steering: The robot's direction is determined by Spike's programming for optimized performance.

•	Driving: It autonomously moves using motors, color sensors, and a proximity sensor. The proximity sensor measures the distance to objects and decreases speed to allow color sensors to identify the detected object, whether it's a wall (black color) or one of the objects (green block or red block), and then performs a specific action.

•	Chassis Design: The lower part of our robot consists of three motors connected to each other using black connectors (Connector peg) with the Large Motor. For the front lower part, we used gears (Double Conical Wheel and Angled Gear Wheel) to connect the wheels, utilizing technic 11m beam and Connector Peg. To position the Large Hub in the upper part, we attached a horizontal technic Frame 7x11 toward the front of the vehicle, and on top of it, a vertical second Technic Frame 7x11 was added. To attach the sensors on the upper front, we used two technic 7m beams to connect the Large Motors to the front wheels, connected to the technic 3m beam using a Connector Peg Friction to secure the sensors. Two pieces of technic frame 5x7 were joined with connectors to attach the sensors, and then two technic 11m beams were attached. With the help of a technic 15m beam, the proximity sensor was connected, and the color sensors were attached alongside the Angle element 135 degrees bar.

Electronics
Sensors: The proximity sensor is used to measure the distance to an object or wall in centimeters. There are two color sensors, one detects red color and triggers a right turn, the other detects green color and triggers a left turn. The Orientation Sensor (Hub) acts as the brain, connecting the motor cables to the Hub, allowing the car to move according to programming.

Speed/Direction Control:

Wiring Diagram:
 
![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/f498add0-901a-4f79-a879-a4aa17485d4b)





Programming
•	Flowchart:
![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/8767ab04-5729-47b9-9173-3bc37a1a75be)

 
•	Strategies: Our main strategy was to ensure that the sensors worked smoothly with the motor and that the robot could autonomously respond to specific colors using the color sensor.









•	Code Discussion:

![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/56824b32-2ef2-4f47-81df-031c64a6367f)
 
The code begins by defining several variables that will be used to store sensor readings, motor speeds, motor positions, and movement commands. Here, the code initializes sensor variables with placeholders for sensor readings. The actual sensor readings would replace these placeholders during the robot's operation. The initial speed and position of the motors are set, and a timer is reset to 0.

![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/0a504f9d-6b54-40ae-9c16-de65962d8e0a)

 
After pressing the right button, the timer resets to zero (0), and subsequently, the code enters a loop that repeats until a certain condition is met. If the distance measured by Sensor_P_B is less than 30 cm, the robot responds by adjusting the motor speeds and positions. The robot turns motor E to a specific position, then motor F is activated for 2 seconds. After that, the robot returns motor E to its initial position and moves motor F in the opposite direction.

![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/4cad2f23-5672-4101-bb57-64dc46ea15e2)

 

If the distance measured by Sensor_P_B is not less than 30 cm, the code checks if it's less than 90 cm. If so, motor E is turned to another position. If not, motor E's position is reset, and motor F moves in the opposite direction to move the vehicle forward. The loop continues until the timer exceeds 50 units in seconds. Finally, the movement of motor F is stopped. This marks the end of the algorithm.

In summary, our Spike algorithm controls a robot's actions based on sensor readings, adjusting motor positions and speeds to respond to detected distances. The robot follows a set of conditions to determine its movements and actions, and repeats these actions until a predetermined time limit is reached.







Daily Log Entry
July 10, 2023: We began assembling and discussing within the team, what the robot's chassis would be.
July 19, 2023: We continued assembling the robot and positioning it.
July 23, 2023: We created the initial programming codes for the vehicle's functionality.
July 26, 2023: Testing Day, and we continued updating the programming, which posed some challenges.
July 31, 2023: The programming with the distance sensors is improving and showing good traction.
August 2, 2023: We added the color sensor. We attempted to combine all three sensors - the proximity sensor and the color sensor.
August 9, 2023: We successfully achieved the vehicle's function and completed the project.

•Challenge and Solution: Our main challenge was integrating the proximity sensor with the color sensor. 

Conclusion
In conclusion, our robot named Indie is capable of autonomous movement and utilizes various sensors including a proximity sensor, two color sensors, and the Hub as the brain, connected to a computer for programming.

Information: The Hub acts as the brain, and the battery is connected.

What motivated us to create this vehicle?
We were inspired by Tesla vehicles for their track record in autonomy.
Mobility: Initially, we drew inspiration from traditional automotive systems, but realizing the space constraints, which were crucial to us, we looked for an alternative. We came up with the idea of using gears, as it was lighter and occupied less space.
Power: We decided to use two motors to handle the robot's weight, enhancing mobility and speed. We incorporated a bar for better precision in vehicle movement.
•	Sensors: The proximity sensor helps Indie measure turning distance, and the color sensors assist in determining the direction of turns based on color.

•	Speed and Direction Control: The motors, in combination with programming, were pivotal for achieving speed and direction control. The two motors determine whether the vehicle turns left or right.

•	Used parts

![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/8671541c-8a4b-49c3-874c-2f5e6ebf6ac7) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/cbf02526-b148-41e3-87cc-ea1533ee7d17) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/aed9c0c1-5196-40de-ac54-d20ac271de95) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/acc3b15f-84a1-467a-a650-9766f07cdf99) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/ff201177-1a3e-4385-8a32-1fea0ebd62fd) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/420d287e-d2f1-4d79-9178-936de39b9c09) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/e41ae3fa-d029-46e0-8f14-f38d8712ac75) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/c618788c-0161-4830-9dc1-63b01466ed3c) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/a773e395-1b2d-401b-9235-9eb7bb1bd369) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/9e01b2fa-b560-447f-93b6-ddb865480c24) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/a9a805cb-ed68-40fa-91f3-b385f7200538) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/13a7ba15-fa4f-48cd-83e2-368d91eb2a4e) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/a1fad93c-cdb8-4acc-a49f-723d517e141d) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/6eac1c3e-dad9-40d6-810b-34538c287554) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/9fc091c2-7f30-4fab-97be-ab4172955405) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/f77a64d0-f386-4eb4-9ef7-9309d0545d2d) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/4d87d4a0-fb24-44ef-a57e-074e304f8209) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/544579fb-06c9-4d4a-8acb-15dcb20dc689) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/4f5946fe-7f0f-481f-8c04-00aca7e4489d) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/9fb952f9-2f13-49dd-bc13-6451c38c74b7) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/69714563-7eb8-49fd-b2d2-2fa548e0c3ad) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/e77fc226-bbc2-4c1f-aeb6-73957fd13f33) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/d4ed32ff-70d1-40ca-8da4-94627b534c38) ![image](https://github.com/ebenz2023/eben-z-aa-wro2023-FE/assets/55847388/7042d48d-797e-4b8e-b1c1-6f8fd0288e56)







              
      

