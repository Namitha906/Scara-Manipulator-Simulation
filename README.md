#  3-DOF SCARA Manipulator Simulation

This project demonstrates the design, kinematic modeling, simulation, and animation of a **3-DOF SCARA manipulator** for pick-and-place operations.

The project applies **inverse kinematics and forward kinematics** concepts to control the motion of the robot arm and simulate a pick-and-place task.

---

##  Project Overview

The SCARA manipulator consists of:
- Two **revolute joints** for planar motion
- One **vertical motion** for pick-and-place

The robot performs the following sequence:
1. Move from home position
2. Move above the object
3. Lower to pick the object
4. Lift the object
5. Move to target location
6. Place the object
7. Return to home position

---

##  Tools Used

- **MATLAB** – Kinematics modeling and simulation
- **Blender** – Robot animation
- **TinkerCAD** – Robot structure design

---

##  Kinematics Used


## Inverse Kinematics

Used to compute joint angles from the desired end-effector position.

**Radial distance**

r = √(x² + y²)

**Joint angle θ₂**

θ₂ = cos⁻¹((r² − L₁² − L₂²) / (2L₁L₂))

**Joint angle θ₁**

θ₁ = tan⁻¹(y/x) − tan⁻¹((L₂ sin θ₂) / (L₁ + L₂ cos θ₂))

###Forward Kinematics

Forward kinematics is used to compute the position of the joints and the end-effector from the known joint angles.

**Position of Joint 1**

x₁ = L₁ cos(θ₁)  
y₁ = L₁ sin(θ₁)

**Position of End Effector**

x₂ = x₁ + L₂ cos(θ₁ + θ₂)  
y₂ = y₁ + L₂ sin(θ₁ + θ₂)

**Vertical Position**

z = z₀ − d₃

---



## Project Videos
Blender Animation
https://drive.google.com/file/d/17988lL8z2UsFo-sG8JUPp_VtmoU9g3qn/view?usp=sharing

Matlab Animation
https://drive.google.com/file/d/1oo6Yf_R95FDTCDt3bYVFuc_upRpWMxoG/view?usp=sharing

##  Applications

- Pick-and-place automation
- Assembly tasks
- Material handling
- Industrial robotics research

---

##  Author

Namitha  
BTech CSE (AI & ML)
