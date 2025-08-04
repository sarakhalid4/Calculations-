# 💡 Torque Calculation for Robot Arm Servos

This document explains the steps to calculate the required torque for each joint in the robotic arm, select suitable servo motors, and provides purchase links.

---

 📏 Arm Lengths
- First arm: 10 cm
- Second arm: 15 cm
- Third arm: 4 cm

---

 ⚖️ Load to Lift
- Target weight: 1 kg
- Generated force: weight × gravity = 1 kg × 9.81 m/s² = 9.81 N

---

 🧮 Torque Calculation for Each Joint

 1️⃣ First Joint (BASE)

- Furthest distance: 10 + 15 + 4 = 29 cm (0.29 m)
- Required torque: Torque1 = 9.81 × 0.29 = 2.84 N·m
- Adding 30% safety margin: 2.84 × 1.3 ≈ 3.7 N·m

 2️⃣ Second Joint (SHOULDER)
- Furthest distance: 15 + 4 = 19 cm (0.19 m)
- Required torque: 9.81 × 0.19 = 1.86 N·m
- Adding 30% safety margin: 1.86 × 1.3 ≈ 2.42 N·m

 3️⃣ Third Joint (ELBOW)
- Furthest distance: 4 cm (0.04 m)
- Required torque: 9.81× 0.04 = 0.39 N·m
- Adding 30% safety margin: 0.39 × 1.3 ≈ 0.51 N·m

  🔧 Suggested Servo Motors and Purchase Links
- First Joint (Torque ≥ 3.7 N·m) 
-   Dynamixel MX-64 or MX-106  
- Example purchase link: [](http://www.robotis.us/mx-64t/)
  
- Second Joint (Torque ≥ 2.42 N·m)
-   Dynamixel MX-28  
-   Example purchase link: [](https://www.mybotshop.de/DYNAMIXEL-MX-28AT-Bulk-6-pcs)
-   
- Third Joint (Torque ≥ 0.51 N·m)**  
-   Dynamixel AX-12A  
-   Example purchase link: [](http://www.robotis.us/ax-12a/)


  🚨 What If We Try to Lift 2 kg?
- Required torques will double:
- Torque1 ≈ 5.68 N·m
- Torque2 ≈ 3.72 N·m
- Torque3 ≈ 0.78 N·m
- The previously suggested servos may not be sufficient for the first and second joints.

  Risks include:
- Servo overheating or permanent damage
- Arm bending or breaking
- Reduced speed and precision
- Excessive power consumption

---

 ✅ Solutions and Alternatives
- Use gears to increase torque (reduces load on the motor)
- Choose stronger servo motors for higher torque
- Shorten the arm lengths to reduce torque requirements
- Use lightweight materials for the arm to reduce self-weight




