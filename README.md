# **WINT 3794 FRC AT HOME 0$ ROBOT IDEA**

The initial idea is to create a competitive robot that can accomplish all FIRST at home challenges with a 0 dollars budget.

The chasis will be the same as WinT 3794 FRC 2020 robot with the only change of pneumatic wheels to HiGrip 6 inches wheels.

The chasis consist of 6 NEO motors (3 per side) chain driven with 2 REV throughBore encoders at the lasts wheels to perform autonomous tasks using differential equations.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Chasis.JPG?raw=true)

Now let's approach how to improve this robot to accomplish all First At Home tasks.

---
# **Galactic Search Challenge**

*"In the Galactic Search challenge, teams emulate the Autonomous Period of INFINITE RECHARGE
gameplay by locating and collecting POWER CELLS as fast as they can on one of two (2) pairs of paths."*

**IMPORTANT RULES**

*"GSC2. Teams must randomly determine (e.g. coin, die, phone app, etc.) if they run the red or blue paths.
Teams make a single random determination and then run the same color on both paths.
The intent is that teams do not signal directly to the ROBOT which option has been
chosen. Placement of the ROBOT is not considered signaling."*

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/PathA%20Galactic.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/PathB%20Galactic.PNG?raw=true)

# What do we need to accomplish this?

In this challenge we need a fast intake to collect the three balls, another thing to have in consideration is robot's center of mass to be able to run at 100% speed without risk, we also need a certain type of feedback to know the position of the robot so it can move to all three positions of the balls consistently and some kind of vision to let the robot know if is going to do red stars or blue stars.

I think the best way to approach this is by keeping a low profile robot, use the already existing REV encoders as position feedback, a passive intake activated with servos due to lack of motors and pneumatic and a webcam with OpenCv to determine whether we are going to do red or blue stars.

---
# Intake Design
To design the intake I consider two main things.

1. The intake needs two rollers to overcome the bumper and move the ball with enough X direction force inside the robot.
1. Needs to be as simple as possible.

For that reason I got this intake design:

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Intake.JPG?raw=true)

This intake is made out of MDF, it has a PVC roller and 16 2.25 inches compliant wheels on top, it is driven through chain and a 775 motor with a 10:1 gearbox.
With this simple robot we should be able to complete challenge #1 and the only thing that is missing is how to deploy the intake without any motor or pneumatic system.

To solve the **how to deploy the intake** problem I used 2 servos to lock the intake and then those servos will be moved to let the intake fall by gravity and elastic rubber bands.
You will understand better with the following images:

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Intake%20Seguros.JPG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/IntakeFRC.gif?raw=true)

Finally I will add a camera on top of the intake to determine which path we will go to play.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Camera.JPG?raw=true)

---
# **AutoNav Challenge**

*"In the AutoNav Challenge teams program their ROBOTS to autonomously drive predetermined routes
through three (3) different paths as fast as possible."*

For this challenge we only need a fast chassis with some encoder feedback, so we must be fine with our actual robot.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Barrel%20Racing%20Path.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Slalom%20Path.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Bounce%20Path.PNG?raw=true)

---
# **Hyperdrive Challenge**

*In the Hyperdrive Challenge teams drive their ROBOTS remotely, without the assistance of preprogrammed navigation, through four (4) different paths as fast as possible. The first three (3) paths are
the same as those described in AutoNav Challenge, the fourth path is the Lightspeed Circuit path.*

To accomplish this challenge we only need a good driver and the robot should work as it is designed now.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Barrel%20Racing%20Path.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Slalom%20Path.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Bounce%20Path.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/LightSpeed.PNG?raw=true)

---

# **Interstellar Accuracy Challenge**

*In the Interstellar Accuracy Challenge teams emulate the shooting challenges of INFINITE RECHARGE
gameplay by scoring POWER CELLS into a representation of the BOTTOM PORT, OUTER PORT, AND
INNER PORT from four (4) zones. Teams will attempt to score as many points as possible in five (5)
minutes.*

**Important Rules**

1. Teams may not attempt more than fifteen (15) POWER CELL shots.
1. Teams must attempt at least three (3) POWER CELLS per zone. The remaining three (3)
POWER CELLS may be shot from any of the four (4) zones.
1. The ROBOT may not be preloaded with more than three (3) POWER CELLS such that they are
fully and solely supported by the ROBOT.
1. No more than two (2) people may feed POWER CELLS to the ROBOT.
1. The ROBOT must be completely within the Reintroduction Zone in order to acquire POWER
CELLS from humans.

**Scoring**

- BOTTOM PORT = 1 Point
- OUTER PORT = 2 Points
- INNER PORT = 3 Points

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Field.PNG?raw=true)

---
# What do we need to accomplish this?

A fast indexer, a fast way for human players to introduce balls, a very accurate shooter and an adjustable angle to be able to shoot from all different 4 spots.

---
# Indexer Design
**Requirements:**

1. It must use only 1 motor.
1. It should be able to keep 3 balls.
1. It should be open for human players to introduce balls as quick as possible. 

The first part of the indexer consist of a conveyor belt in the floor to transport balls.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Caminadora.JPG?raw=true)

The conveyor belt will be built with **Home Depot** Non-slip tape.

![](https://cdn.homedepot.com.mx/productos/723546/723546-z.jpg)

Then the second part of the indexer consist of side conveyors to center the ball at the end.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Indexer.JPG?raw=true)

Finally I will add the motor and the needed gears to make it run.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Motorized.JPG?raw=true)

---

# Shooter Design
**Requirements:**

1. It must use 4 motors.
1. It should be able to shoot in the opposite direction of the intake.
1. It should have an adjustable angle. 

The shooter consist of a 4 inches compliant wheel roller at the bottom to transport balls from indexer toward flywheel, the flywheel has 4 775pro 1:1 geared motors with an external 2:1 reduction that we can change if we need, then we have 4 inches colson wheels to shoot the balls at a teorethical speed of 9000rpm and finally an adjustable shooting angle driven by 2 servos.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Completedv1.JPG?raw=true)

Finally I added the limelight and a logo of the team.

![]()

![]()

![]()