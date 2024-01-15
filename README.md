# BaseSwerve
[![CI](https://github.com/Pearadox/BaseSwerve/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/Pearadox/2024AlphaBot/actions/workflows/main.yml)

Swerve drive implementation that can be used as a starting point for programming a swerve drive robot.

Action Items:
1) Document the exact dimensions and hardware installed on our base robot (26x26, sparkmax, pigeon, etc.)
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
6. 26x26 base

Software specifications:
1. SwerveKinematics order: LeftFront, RightFront, LeftBack, RightBack
=======
