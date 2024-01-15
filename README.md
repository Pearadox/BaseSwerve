# BaseSwerve
[![CI](https://github.com/Pearadox/BaseSwerve/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/Pearadox/2024AlphaBot/actions/workflows/main.yml)

Swerve drive implementation that can be used as a starting point for programming a swerve drive robot.

 Action Items:
2) Document all the key elements of configuring the swerve drive.
3) Document all the key elements of troubleshooting the swerve drive.
4) Update the code to have all the key elements output to the Smart Dashboard in a usable fashion.

 Vendor Dependencies:
1) https://software-metadata.revrobotics.com/REVLib-2024.json
2) https://maven.ctr-electronics.com/release/com/ctre/phoenix6/latest/Phoenix6-frc2024-latest.json
3) https://3015rangerrobotics.github.io/pathplannerlib/PathplannerLib.json

 Hardware and dimensions:
1. CANSparkMax for drivetrain
2. CTRE Pigeon 2.0 gyro
3. CANcoder
4. Double Neo
5. SDS Mk4i L2 Swerve Module
6. 26x26 base - 20.75 inches for both track width and wheel base
7. 4 in diameter wheels

 Software specifications:
    - SwerveKinematics order: LeftFront, RightFront, LeftBack, RightBack

 Offsets for swerve angles:
1. Download Phoenix Tuner X
2. Plug into RoboRio with USB A to B
3. Click on each CANcoder
4. Turn all the wheel to the forward position
5. Hit refresh, and record the absolute positions as Constants
6. Name each swerve offset in the format of: LEFT_FRONT_OFFSET
7. Make sure the wheels are oriented in the correct direction 
8. Turn 180 degrees if not (turn on its side to test); you'll know if its in the correct direction by driving
9. Make sure each encoder and motor are inverted if needed
10. Each swerve module orientation is forward positive and counter-clockwise positive

##### Glossary:
    - Slew rate limiter -- softens the behavior of control inputs by capping the maximum rate of change
    - Kp Tuning constant -- the most important part of the PID loop/controller
    
[FRC 0 to Autonomous](https://youtu.be/0Xi9yb1IMyA) tutorial on how to program swerve