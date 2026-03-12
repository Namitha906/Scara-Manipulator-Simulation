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

### Inverse Kinematics

Used to compute joint angles from the desired end-effector position.

\[
r = \sqrt{x^2 + y^2}
\]

\[
\theta_2 = \cos^{-1}\left(\frac{r^2 - L_1^2 - L_2^2}{2L_1L_2}\right)
\]

\[
\theta_1 = \tan^{-1}\left(\frac{y}{x}\right) -
\tan^{-1}\left(\frac{L_2\sin(\theta_2)}{L_1 + L_2\cos(\theta_2)}\right)
\]

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
