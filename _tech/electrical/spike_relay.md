---
title: Spike Relay
tags: aux-cs
---

The Spike Relay has been a part of FRC since 2000. It was provided in all KOPs from 2000 to 2014 and was still legal from 2015 to 2017.

## Data

The [Robot Controller](robot-controller) sends a Relay signal to the Spike. When it receives a FWD signal, it applies +12v to M+ and grounds M-. Likewise when it receives a REV signal, it applies +12v to M- and grounds M+. When both signals are received, +12v is applied to M+ and M- and nothing is grounded.


## Connections


### Motors

Spikes can be connected to a [motor](motor) that does not need to move at a variable speed. The motor cannot draw more than 20A.


### Solenoids

Spikes can be connected to one or two solenoids. To connect two solenoids simply ground the negative ends of the [solenoid](solenoid) to the grounding portion of the [power distribution board](power-distribution-board) and the positive ends to M+ and M-.


### Air Compressor

The air compressor can also be connected to the Spike, but care should be taken to always observe the proper polarity. The NEG output should never be enabled. If the compressor is powered in reverse, it will appear to function, but it will be drawing more current and producing more heat than it should for the amount of air it moves. Also, note that FIRST recommends that you remove the spike module's 20 amp fuse and replace it with a 20 amp circuit breaker to avoid nuisance blowing of the fuse when the spike module is used with an air compressor.


### Pinout of Control Input

The control input to the Spike relay is a three-pin receptacle where a three-wire cable from the [Robot controller](robot-controller) is connected to. The black wire is grounded.

When the white wire is at +5V and the red wire is at 0V, M+ receives the full input voltage. When the red wire is at +5V and the white wire is at 0V, M- receives the full input voltage.

## Kit of Parts

### 2015-2017

The Spike Relay is legal for use, but is not provided in the KOP.

### 2013-2014

One Spike Relay is provided to all teams.

### 2010-2012

One Spike Relay is provided to all teams, with one additional relay provided to rookie teams only.

### 2009

Two Spike Relays are provided in the KOP.

### 2001-2008

Four Spike Relays are provided in the KOP.

### 2000
The Spike Relay makes its debut in FRC. Four are provided in the KOP


#  Spike Red

Occasionally you might see versions of the Spike relay floating around that have red lettering. These are older editions of the relay and lack reverse polarity protection on their inputs. In addition, when no control signal is present, the M+ and M- pins are connected to +12 instead of GND (So a 0 in software is +12, and a 1 in software is a GND)

# Manuals
[Spike Blue Manual](https://web.archive.org/web/20030419143006/http://www.innovationfirst.com/FirstRobotics/pdfs/SpikeBLUEUsersManual.pdf "https://web.archive.org/web/20030419143006/http://www.innovationfirst.com/FirstRobotics/pdfs/SpikeBLUEUsersManual.pdf")  
[Spike Installation Info](https://web.archive.org/web/20030323140520/http://www.innovationfirst.com/FirstRobotics/pdfs/SpikeInstallationInfo.pdf "https://web.archive.org/web/20030323140520/http://www.innovationfirst.com/FirstRobotics/pdfs/SpikeInstallationInfo.pdf")
