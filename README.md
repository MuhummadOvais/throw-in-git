# Robotic Arm Throwing Simulation

## Overview

This project simulates a robotic arm in Webots that picks up an object and performs a controlled throwing motion. The goal is to demonstrate joint coordination, object manipulation, and physics-based interaction within the Webots environment.

---

## Robot Setup


The robot consists of:

- 3 Degrees of Freedom (DOF):
  - Shoulder joint (controls horizontal movement):
  - Elbow joint (controls arm bending):
  - Wrist joint (controls the final arm rotation):
  
  - End Effector:
    A gripper for object pickup and releasekup and release

---

## Environment

- Platform: Webots
- Flat arena with physics enabled
- A RoboCup ball as the target object

---

## Devices Used

- Rotational Motors:
  - Shoulder motor
  - Elbow motor
  - Wrist motor

- Gripper:
  - Used for grabbing and releasing the object (RoboCup ball)

---

## Implementation

The robot follows a sequence-based control approach:

1. Rotate the shoulder joint to align with the ball
2. Move the arm to the pickup position using the elbow joint
3. Close the gripper to pick up the ball
4. Lift the ball by controlling the shoulder, elbow, and wrist joints
5. Perform a backswing motion
6. Execute throw
7. Release the ball by opening the gripper

Control is implemented using:
- `setPosition()` for joint control
- Timed steps for smooth motion execution

---

## Challenges

- Aligning the robot with the ball accurately
- Positioning the gripper correctly above the ball for pickup
- Ensuring smooth coordination between joints for the throwing motion
- Tuning joint angles for realistic movement and ball release

---

## Final Result

The robot is able to:
- Align itself with the ball
- Pick it up using the gripper
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
