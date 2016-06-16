---
title: Servo
tags: aux-cs
---

{% include wikilink topic="Servomechanism" %}

A **servomechanism**, usually called a **servo** is like a [motor](Motor "Motor"), expcept that it's axle goes to a specific place instead of just spinning. They are connected to the [robot controller](robot-controller) through a [PWM](pwm) interface.

## Continuous Rotation Servo

A Continuous Rotation Servo is a servo capable of rotation past 360°. This allows one to use a continuous rotation servo as a small motor. Such servos are capable of only full forward, stopped, or full reverse motion. Most servos of this type are controlled by a [PWM](pwm) signal whose width controls the rate of turn.

## Standard Rotation Servo

Most servos are capable of only 90, 180, or 270 degrees of rotation. Such servos are used for accurate angular positioning of a mechanism. Most servos of this type are controlled by a [PWM](pwm) signal whose width controls the angular position of the servo.
