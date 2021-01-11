# WINT 3794 FRC AT HOME 0$ ROBOT IDEA

The initial idea is to create a competitive robot that can accomplish all FIRST at home challenges with a 0 dollars budget.

The chasis will be the same as WinT 3794 FRC 2020 robot with the only change of pneumatic wheels to HiGrip 6 inches wheels.

The chasis consist of 6 NEO motors (3 per side) chain driven with 2 REV throughBore encoders at the lasts wheels to perform autonomous tasks using differential equations.

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/Chasis.JPG?raw=true)

Now let's approach how to improve this robot to accomplish all First At Home tasks.

---
# Galactic Search Challenge

"In the Galactic Search challenge, teams emulate the Autonomous Period of INFINITE RECHARGE
gameplay by locating and collecting POWER CELLS as fast as they can on one of two (2) pairs of paths."

IMPORTANT RULES

"GSC2. Teams must randomly determine (e.g. coin, die, phone app, etc.) if they run the red or blue paths.
Teams make a single random determination and then run the same color on both paths.
The intent is that teams do not signal directly to the ROBOT which option has been
chosen. Placement of the ROBOT is not considered signaling."

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/PathA%20Galactic.PNG?raw=true)

![](https://github.com/PaoloReyes254/FRC_At_Home_2021/blob/master/Images/PathB%20Galactic.PNG?raw=true)

# What do we need to accomplish this?

In this challenge we need a fast intake to collect the three balls, another thing to have in consideration is robot's center of mass to be able to run at 100% speed without risk, we also need a certain type of feedback to know the position of the robot so it can move to all three positions of the balls consistently and some kind of vision to let the robot know if is going to do red stars or blue stars.

I think the best way to approach this is by keeping a low profile robot, use the already existing REV encoders as position feedback, a passive intake activated with servos due to lack of motors and pneumatic and a webcam with OpenCv to determine whether we are going to do red or blue stars.