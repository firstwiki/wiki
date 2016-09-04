---
title: Dead Reckoning
tags: programming
---

{% include stub %}
{% include cleanup %}

**Dead reckoning** refers to a system operating without awareness of its absolute position. Instead, path integration is used based on a previous known location. In [FIRST](first), [robots](robot) may use dead reckoning if they do not have [sensors](sensor) to measure absolute position (for example, rangefinders). Dead reckoning can be used in [autonomous mode](autonomous-mode) to track approximate robot field position for autonomous operations. Accuracy depends on the rate of the integration loop as well as the accuracy of the [sensors](sensor), and error accumulates over time.

One method of dead reckoning uses a [gyroscope](gyroscope) and [encoders](encoder) to track 2D field position. On each step, the robot can integrate its current position from its starting position by advancing the position by the change in the [encoder](encoder) value in the direction measured by the [gyroscope](gyroscope) value.
