
# 🤖 Robotics Lab: 3-Tier Tower of Hanoi with ABB RobotStudio®

Welcome to our Robotics Lab Project! This repository documents our work on solving the **3-Tier Tower of Hanoi** problem using **ABB IRB 120** industrial robot simulated in **ABB RobotStudio®**. 🏗️🧠

---

## 🧩 Project Objective

To design, simulate, and optimize a pick-and-place system using **ABB RobotStudio®** to solve the 3-block Tower of Hanoi puzzle while achieving the **shortest execution time** under nominal robot operating conditions.

---

## 🏛️ Team Members

👤 Ahmed Abdulgader Salim Assagaf  
👤 Mazen Mohamed Mahrous  
👤 Omar Awad Abdelhadi Mahmoud  
👤 Omar Walaa Hasaan Mohamed Hassan Elmaasri  

Faculty of Electrical Engineering, Universiti Teknologi Malaysia  
FKE, UTM, 81310 Skudai, Johor

---

## 🧠 Understanding Tower of Hanoi

The Tower of Hanoi is a mathematical puzzle consisting of **three blocks** arranged on one peg in decreasing size (3 at the bottom, 1 at the top). The goal is to move all blocks to another peg, following these rules:

1. 🔁 Only one block can be moved at a time.
2. ✋ Each move takes the **top block** from one peg and places it on another.
3. 🚫 No block can be placed on a **smaller block**.

---

## 🛠️ Software & Tools

- 💻 **ABB RobotStudio®**
- 🦾 **ABB IRB 120 (3kg, 0.58m reach)**
- 🛠️ RAPID Programming Language
- 🧩 Smart Components (Gripper simulation)
- 📹 [Simulation Video on YouTube](https://youtu.be/43ik-pjxENo)

---

## 🧪 Procedures

The project followed these general steps:

1. 📦 Created new solution in RobotStudio with **Virtual Controller**.
2. 🏗️ Imported and arranged station components and IRB 120 robot.
3. ✋ Attached **MyGripper** tool and created **work objects** and targets.
4. 🔄 Used **MoveJ**, **MoveL**, and **MoveC** instructions to define trajectories.
5. 🧠 Optimized orientation and approach/depart positions.
6. 💡 Created **Smart Components** and connected I/O signals.
7. 🎛️ Synchronized RAPID ⇄ Station, configured motion types & velocity.
8. ▶️ Ran simulations and optimized for shortest execution time.

---

## 💡 Motion Types in RAPID

| Motion Type | Path | Use Case |
|-------------|------|----------|
| `MoveJ`     | Non-linear (joint-based) | Fast positioning, no obstacle awareness |
| `MoveL`     | Linear                  | Precise straight-line movement |
| `MoveC`     | Circular                | Arcs or full circular paths |

📌 **RAPID Syntax Example:**
```rapid
MoveL pTarget, v100, fine, toolGripper\WObj:=wobj0;
```

---

## 📊 Results

Despite initial software compatibility issues and lag, we successfully:

- 🧩 Solved the Tower of Hanoi using pick-and-place simulation
- ⏱️ Achieved an **optimized runtime of 29.2 seconds**
- ✅ Demonstrated proper use of MoveJ, MoveL, and MoveC
- 🛠️ Built complete RAPID code and Smart Component configuration

---

## ⚠️ Challenges Faced

- 🔄 Firmware compatibility issues with older robot version
- 🐢 Software lag affecting movement precision
- 🧯 Frequent safety/access errors during simulation

Sample error:
```
Error in T_ROB1 - Module1 - Line 103.
Two channel fault, RUN CHAIN.
The operation was rejected by the controller safety access restriction mechanism.
```

---

## 🎯 Learning Outcomes

✔️ Understood and implemented trajectory planning  
✔️ Gained experience with ABB RobotStudio® and IRB 120  
✔️ Practiced RAPID programming with motion instructions  
✔️ Learned how to simulate realistic industrial robot tasks

---

## 📎 Appendix

📁 `SimulationFiles/` - Contains RobotStudio `.rspag` file  
📁 `RAPID/` - Contains `.mod` file with final working code  
📽️ [Watch our final simulation](https://youtu.be/43ik-pjxENo)

---

