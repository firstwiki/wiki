---
title: PWM Cable
tags: communication
---

{% include outdated-warning %}

A PWM Cable is a 3-pin cable with a connector on each end designed to plug into
both the [robot controller](robot-controller) and the [Victor 884](victor-884)
speed controller. This cable carries a [PWM](pwm) signal.


## Other Uses of the PWM Cable

The PWM cable is not designed specifically for PWM signals and is only known
as a "PWM Cable" colloquially and only in the hobby robotics community. These
cables can be used for the serial connection from the 2005 IFI breaker board,
allowing it to communicate with the robot controller. It can also be used for
the serial connection on the cmu2cam. [Spike relays](spike-relay) also use a
3-pin cable identical to the [Victor 884](victor-884), as do many sensors.


## Other Types of Cables Used for PWM Signals

Many teams have stopped using these 3-pin cables, citing the difficulty in
installing and removing so many cables, as well as the tendency of the cables to
spontaneously disconnect from the [robot controller](robot-controller). These
teams have begun using large, multipin cables that they have attached custom
connectors to allow them to connect to the [robot controller](robot-controller)
and [Victor 884](victor-884). These cables include ribbon cables
of the type used for computer disc drives and DB-9 type cables used in PC serial
cables. By using these types of cables, there are fewer wires to organize and a
quick-disconnect can be installed to facilitate modular/removable electronics
panels.
