#The Tale of Interconnected Pendulums

For this task, we had to build a Simulink model depicting an interconnected pendulum apparatus and design a control system governing the motion of Lumina(1) using a control input u(t) while allowing Ignis’s motion(2) to adapt naturally based on relative displacement(2 - 1).

I built a Simulink model using the following equations:

I1(1)'' + b1(1)' + k11=u(t)

I2(2)'' + b2(2)' + k22=k2(2-1)+d

I used the Ziegler-Nichols method to tune the controllers manually.
For zero initial conditions, I built a P, PI, and PID controller and compared their response and error graphs to decide which one is best.
The disturbance torque is a sinusoidal wave of amplitude 5cm and frequency 100 radians/sec.
