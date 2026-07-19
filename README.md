## **initial Design of a RobotDog focuses on studying and analyzing the mechanical fundamentals enabling the robot to stand and walk.**


# **RobotDesign**

1. Body and Frame Shape

The robotic dog has a quadruped (four-legged) design inspired by a medium-sized dog. The body consists of a lightweight aluminum frame covered with durable ABS plastic panels. The battery, controller, and sensors are placed inside the body to keep the center of gravity low and improve stability.

# **Specifications**

Length: 60 cm
Width: 25 cm
Height: 40 cm
Weight: 8 kg
2. Leg Design

The robot has four identical legs, each designed to imitate the movement of a real dog's leg.

**Each leg consists of:**

Hip joint
Upper leg
Knee joint
Lower leg
Ankle joint
Rubber foot for grip

This design allows the robot to walk, climb small obstacles, and maintain balance.

3. Number of Joints and Degrees of Freedom (DOF)

Each leg has 3 Degrees of Freedom (DOF):

Hip Yaw (side movement)
Hip Pitch (forward/backward movement)
Knee Pitch (leg bending)

Total DOF:

4 Legs × 3 DOF = 12 DOF

Optional:

Head rotation = 2 DOF
Tail movement = 1 DOF

Total = 15 DOF

4. Motor Selection

The robot uses high-torque servo motors for precise joint control.

# **Recommended motors:**

Dynamixel XL430
MG996R (low-cost prototype)
Robotis Dynamixel XM430 (advanced version)

# **Motor requirements:**

High torque
Position feedback
Fast response
Low power consumption
5. Torque Calculation for One Joint

Assume:

Robot weight = 8 kg
Weight supported by one leg = 2 kg
Leg length = 0.18 m

Force:

F=m×g
F=2×9.81=19.62 N

Torque:

T=F×L
T=19.62×0.18
T=3.53 N⋅m

Required motor torque ≥ 4 N·m (including a safety factor).

# **6. Stability and Center of Gravity**

The center of gravity (CoG) is positioned near the middle of the robot's body and kept as low as possible by placing the battery and electronics in the lower section of the chassis.

To improve stability:

Wide stance between the four legs
Low center of gravity
Rubber feet for better traction
Even weight distribution

The robot remains stable as long as the center of gravity stays within the support polygon formed by the legs touching the ground.

# **7. Walking Method**

The robot uses a Trot Gait.

Walking sequence:

Front Left + Rear Right move together.
Front Right + Rear Left move together.
Repeat the cycle.

# **8. Expected Mechanical Problems**

Servo motor overheating during continuous operation
Joint wear after long-term use
Reduced traction on smooth surfaces
Battery drain during high-speed movement
Leg vibration at high walking speeds
Frame deformation under heavy loads
Cable damage due to repeated joint motion
Loss of balance on uneven terrain
