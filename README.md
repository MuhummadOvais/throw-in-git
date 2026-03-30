# Vacuum Gripper Throwing Robot

## Overview
This project simulates a robotic arm in Webots that uses a vacuum gripper to pick up an object and perform a controlled throwing motion. The goal is to demonstrate joint coordination, object manipulation, and physics-based interaction.

---

## Robot Setup

The robot consists of:

- 3 Degrees of Freedom (DOF):
  - Yaw joint (base rotation)
  - Pitch joint (shoulder movement)
  - Roll joint (elbow movement)

- End Effector:
  - Vacuum gripper for object pickup and release

---

## Environment

- Platform: Webots
- Flat arena with physics enabled
- Cardboard box as target object

---

## Devices Used

- Rotational Motors:
  - yaw motor
  - pitch motor
  - roll motor

- Vacuum Gripper:
  - Used for attaching and releasing the object

---

## Implementation

The robot follows a sequence-based control approach:

1. Rotate base to face the object
2. Move arm to pickup position
3. Activate vacuum gripper
4. Lift the object
5. Perform back swing motion
6. Execute throw
7. Release object

Control is implemented using:
- `setPosition()` for joint control
- Timed steps for motion execution

---

## Challenges

- Aligning robot with object position
- Positioning gripper correctly above the object
- Ensuring proper suction timing
- Tuning joint angles for realistic motion

---

## Final Result

The robot is able to:
- Align itself with the object
- Pick it using a vacuum gripper
- Perform a throwing motion
- Release the object using simulation physics

---

## How to Run

1. Open Webots  
2. Load: `worlds/throw_prototype.wbt`  
3. Run the simulation  

---

## Future Improvements

- Add camera-based object detection  
- Implement inverse kinematics (IK)  
- Improve throwing accuracy  
- Add sensors for feedback control  

---

## Author
Muhummad Ovais
