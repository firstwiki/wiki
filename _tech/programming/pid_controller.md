---
title: PID Controller
---

A **Proportional-Integral-Derivative controller** is a [closed loop](closed-loop) [feedback](feedback) control. It is used to get some device to reach a _setpoint_ by reacting based on the [error](error) of the system. The [program](programming) reads in [input](input) from a [sensor](sensor) and reacts based on the difference between the sensor reading and the setpoint (the desired sensor reading) in three ways.

- The error is multiplied by a **proportional** constant P. This handles the present, basing the output proportionally on the error.
- The error is integrated (or summed) over a time period and then multiplied by an **integral** constant I. This handles the past, basing the output on how long the error has persisted.
- The first derivative of the error (its rate of change, often the difference between the current and previous error is used) is calculated with respect to time and then multiplied by a **derivative** constant D. This handles the future, basing output on how quickly the error is changing.

The sum of these calculations is then added to the last [output](output) of the PID loop.

## Theory

_Control_ refers to applying input (e.g., sensor readings) to cause a certain system to conform to desired values (e.g, having an "arm" move to some position). [Open loop](open-loop) control does not use feedback, meaning it does not continuously update its input. [Closed loop](closed-loop) control continuously measures the system variables and corrects the output based on this feedback. Closed loop control adjusts to a dynamic environment where everything is not known exactly. PID control is a specific type of closed loop control, and adjusts the output using proportional, integral, and derivative terms. It is based on control theory, heavy in mathematics (it is actually a differential equation), and is a widely used filter mechanism. For most applications related to [FIRST](first), simplified results of control theory can be used without needing to know advanced mathematical equations.

The general equation for proportional control is

    Pout = Kerr*Kp

where Pout is the output, Kerr= Target value-Current value, and Kp is the gain value.

## Application

PID control is very useful in robotics. It is a way to make sure that what is supposed to happen actually happens, despite a changing environment that can't be controlled. For instance, PID control might be applied to driving the robot, to compensate for wheel slippage and running into obstacles that offer resistance or it might be applied to an "arm" to make it move to the desired position and then resist backdrive due to gravity. There is no shortage of applications. Almost wherever a sensor is used, a PID loop _could_ add for additional control. However, it is not always desirable. It increases the code's complexity and creates at least three constants that must be finely tuned (see below). Also, if the sensor fails, called "going open loop," very undesirable results can happen, depending on how the sensor failed (see below). Despite these disadvantages, though, a PID control can be beneficial to a wide variety of applications. For something that cannot be known fully beforehand [dead reckoning](dead-reckoning) does not work well; but, this is exactly where PID control shines. If, for instance, a robot has a tendency to veer toward some direction besides straight, using [wheel encoders](encoder) and PID control would be able to correct the problem.

It is worth mentioning that many systems are simple enough that a full PID loop is not needed. Often a simple P loop (based solely on proportional control, where I=D=0) is sufficient. Factors such as the speed that the system can respond, the granularity of input, and the expected amount of disturbances affect this, and if these are changed, more advanced control may then be needed. A general rule of thumb in all of engineering is to start out simple, and only add complexity where it is absolutely necessary. Complex things are hard to fix and tend to break more easily. Simple things are much easier to develop.

## Tuning

A PID loop is useless without the correct constants. If these are too high or too low, the system might overshoot drastically, leading to an uncontrolled oscillation. The constants (P, I, and D) may be determined empirically, or calculated if a system model is available for the controlled system. Tuning of a PID loop is an art or skill, which is generally acquired through practice. One suggestion is to start with just P control (I = D = 0). Observe the system response to a small input step command. Increase P until the system just starts to oscillate, meaning it reaches the target (setpoint), overshoots, returns, undershoots and repeats this process; this is so-called _underdamped_ behaviour. Increase D until this oscillation stops; the control should be smoother now, but if increased too far may cause sluggish system response (i.e. the system is _overdamped_). Ideally, step response should have some overshoot, and undershoot, but should settle into the desired setpoint quickly. This may be achieved by repeatedly adjusting P & D until the desired step response is achieved. Integral gain (the I constant) is required if there is some following error in the system; that is, if the controlled variable has a constant difference from desired setpoint. Integral gain should only be used sparingly since it tends to destabilize a system.

## Going open loop

"Going open loop" refers to a closed loop control that loses its input. This might happen because the sensor becomes jostled out of the input slot on the [Robot Controller](robot-controller), wear and tear (aided by walls and opposing robots many times), the [PWM cable](pwm-cable) fails, or some other problem. If the sensor is damaged and the system is not at the setpoint, it will try to reach the setpoint as per the control, but the computer will never think it has reached the setpoint since it is getting an incorrect and non-updated value. This is mentioned because it can be a **safety risk** on certain systems, causing an arm, for instance, to flail about wildly, damaging the robot, passers-by, or both. If strange behavior is observed on a previously working control loop, check the sensors to make sure the correct values are being read, and that the sensor is functioning.

## Positive Feedback

A common mistake when implementing a closed-loop controller is to use the "wrong sign" when subtracting the feedback signal from the setpoint signal. We want negative feedback; i.e. the error signal (setpoint minus the feedback) times the PID gains should lead to a further reduction in the error. Positive feedback will cause a runaway condition that can be very violent, causing damage to people or equipment.

## Safety Mechanisms

In light of the above mentioned issues, a control system designer must always consider the possibility of a sensor failure or other potential fault condition. Steps should be taken in the control system design to limit the motion (or other controlled variable), i.e. position, speed, acceleration of a controlled system. Such controls may be implemented in hardware (e.g. [limit switches](limit-switch)) or software ("soft" limits). If only software limits are available, there should be a watchdog circuit with safe shutdown implemented, since the sanity of the control software cannot be depended upon.

## See also

- [Sensors](sensor)
- [Feedback](feedback)
- [Open loop](open-loop)
- [Closed loop](closed-loop)

## External Links

- [PIDlab.com](http://www.pidlab.com "http://www.pidlab.com") - PID controller laboratory - free Java applets for PID tuning
- See [PID controller](http://www.wikipedia.org/wiki/PID_controller "wikipedia:PID_controller") for more information
- Larry Barello gives a description of various robots he has worked on, and an overview of [PID control](http://www.barello.net/Papers/Motion_Control/index.htm "http://www.barello.net/Papers/Motion_Control/index.htm") (scroll down, code included)
- Several [ChiefDelphi](chiefdelphi) threads related to this issue: ([[1]](http://www.chiefdelphi.com/forums/showthread.php?t=24340 "http://www.chiefdelphi.com/forums/showthread.php?t=24340"), [[2]](http://www.chiefdelphi.com/forums/showthread.php?t=27978 "http://www.chiefdelphi.com/forums/showthread.php?t=27978"))
