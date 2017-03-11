---
title: Aim High
tags: frc_games
---
{% include TODO %}

{% include wikilink topic="Aim High" %}

## Index of FRC Games

- 2011 [Rebound Rumble](Rebound_Rumble "Rebound Rumble")
- 2011 [Logo Motion](Logo_Motion "Logo Motion")
- 2010 [Breakaway](Breakaway "Breakaway")
- 2009 [Lunacy](Lunacy "Lunacy")
- 2008 [FIRST Overdrive](FIRST_Overdrive "FIRST Overdrive")
- 2007 [Rack 'n' Roll](Rack_%27n%27_Roll "Rack 'n' Roll")
- 2006 **Aim High**
- 2005 [Triple Play](triple-play)
- 2004 [FIRST Frenzy: Raising the Bar](FIRST_Frenzy:_Raising_the_Bar "FIRST Frenzy: Raising the Bar")
- 2003 [Stack Attack](Stack_Attack "Stack Attack")
- 2002 [Zone Zeal](Zone_Zeal "Zone Zeal")
- 2001 [Diabolical Dynamics](Diabolical_Dynamics "Diabolical Dynamics")
- 2000 [Co-Opertition FIRST](Co-Opertition_FIRST "Co-Opertition FIRST")
- 1999 [Double Trouble](Double_Trouble "Double Trouble")
- 1998 [Ladder Logic](Ladder_Logic "Ladder Logic")
- 1997 [Toroid Terror](Toroid_Terror "Toroid Terror")
- 1996 [Hexagon Havoc](Hexagon_Havoc "Hexagon Havoc")
- 1995 [Ramp n' Roll](Ramp_n%27_Roll "Ramp n' Roll")
- 1994 [Tower Power](Tower_Power "Tower Power")
- 1993 [Rug Rage](Rug_Rage "Rug Rage")
- 1992 [Maize Craze](Maize_Craze "Maize Craze")

**Aim High** was the name of the 2006 season [FIRST](first) [game](frc-games "FRC Games").

## Contents

- 1 Game Description

  - 1.1 Game Hint

- 2 Field Layout

  - 2.1 Alliance Station

- 3 Tournament Structure
- 4 Kit of Parts
- 5 Rules
- 6 Robots
- 7 Sources

--------------------------------------------------------------------------------

## Game Description

Aim High is played by two alliances, red and blue, each consisting of three robots. During a 10 second autonomous mode, robots will be programmed to score into any of the three goals: one raised center goal marked by a green vision target and two corner goals at floor level. At the end of the autonomous period, the alliance with the most points will gain a 10 point bonus and will be placed on defense for round two. Rounds two, three, and four, which are each 40 seconds long, are human-controlled rounds. Between rounds two and three, the alliances will switch from offense to defense, or from defense to offense accordingly. At the start of round 4, any alliance can score into their corresponding goals. At the end of the match, an alliance can receive bonus points by placing its three robots on a platform below the center goal. The alliance with the most points wins. Scoring will be as follows: 3 points for any ball scored in the center goal, 1 point for any ball scored in the corner goals; 10 bonus points for scoring the highest in the autonomous round; and 25 points for placing all 3 robots on the platform at the end (10 for 2 and 5 for 1).

### Official Game Summary [[1]](https://web.archive.org/web/20150316194933/http://www3.usfirst.org/sites/default/files/uploadedFiles/Who/FIRST_History/FRC_Game_Summaries_Photos.pdf "https://web.archive.org/web/20150316194933/http://www3.usfirst.org/sites/default/files/uploadedFiles/Who/FIRST_History/FRC_Game_Summaries_Photos.pdf")
In the 2006 game, “Aim High,” students’ robots are designed to launch balls into goals while human players enter balls into play and score points by throwing/pushing balls into corner goals. Extra points are scored by robots racing back to their end zones and climbing the ramp to the platform before the end of the 2 minute and 10 second match. 

### Game Hint

FIRST sent this e-mail blast:

> Greetings Teams:
>
> The Game Design Committee is pleased to provide you with the following game clue:
>
> ```
> five 'bots tangling with pasta
> a game piece obsessed with a shovel's show
> and seeing Montana's green heights
 ```
>
> We wish you all a Happy Holiday Season and look forward to seeing you at Kickoff.
>
> Go Teams!

## Field Layout

The Aim High field has 6 goals and 2 platforms. Unlike previous years, an alliance's goals are on the far side of the field. The field is flat, measuring 54 feet long by 26 feet wide.

### Alliance Station

The alliance station wall is 26 feet long and stretches the width of the field. In the middle 18 feet of the alliance station wall exists diamond plate aluminum from the floor to 3 feet high, with clear acrylic filling the rest of the 3 1/2 feet. The outer edges of the wall consist of transparent polycarbonate. Above each alliance station, there is a circular goal (the center goal), with a green light above it. The green light is used so that the CMUCam2 can lock onto it. On the bottom left and right of each alliance station, there are two rectangular holes (the corner goals) through which balls can be scored. In front of each alliance station there is a raised platform.

## Tournament Structure

The tournament structure of this competition is the same as in previous years. In the regional comptitions, teams will be given access to their robots on the Thursday of the competition weekend. It is a day dedicated to practice, giving each team a number of practice rounds on the regulation playing field. Friday and the morning of Saturday is dedicated to a series of qualification rounds. Each team will compete in around seven to ten matches. The number of wins by a team in these matches determines the team's ranking.

Before the lunch break on Saturday, the top eight teams after the qualification rounds are asked to select an alliance of three robots. The order to this selection process goes in order from the top-seeded team to the eight seed. In contrast to previous years, the order reverses for the second selection round; the eighth seed picks first and then backwards in order to the first seed. This was instituted to make the finals more competitive and balanced compared to previous years.

After the lunch break, the finals take place. This is a standard-elimination tournament bracket, starting with alliance 1 facing alliance 8, alliance 2 facing alliance 7, and so on. At the end of the finals, the last remaining alliance is declared the winner and all three teams are given the right to attend the national competition.

## Kit of Parts

There were several changes in the [kit of parts](Kit_of_parts "Kit
of parts") this year,

- The inclusion of the [National Instruments](national-instruments) [LabVIEW](LabVIEW) program
- CMUCam II, including a pan/tilt assembly with [servos](servo), designed to follow an illuminated target
- A new robot controller, based on the PIC18F8722, instead of the PIC18F8520
- New EasyC programming tool
- New, wider CIM motors with drive belts
- New, smaller Window motors
- A new, smaller and lighter backup battery charger
- An IR transmitter and reciever (for broken beam detection)
- And (probably the most surprising) a [digital camera](digital-camera) and _Picasa_ software supplied by [Google](google)

## Rules

Major Rules include:

- Intentionally damaging another robot or the playing field is not allowed.
- No balls may exit the robot at a velocity greater than 12 m/s (39 ft/s).
- The shooter mechanism must remain within the original starting dimensions.
- No part of the robot may ever extend more than 60 inches above the floor.
- If a robot is more then 60 inches high, and it blocks a ball from being shot, a 5 point penalty per ball will be assesed.
- Power supplies are limited to compressed air, a 12-volt motorcycle battery, a 7.2-volt RC battery, deformation of parts (such as springs), and potential energy due to gravity.

## Robots

It is expected that many robots will launch the foam ball with a baseball pitcher mechanism or other shooting mechanism. These will consist of one or two spinning disks that will propel the ball through a barrel and into the goal. Other mechanisms to fire the projectiles might include pneumatic devices or catapults.

The game is a test of accuracy and efficient use of resources, such as the CMUCam, to make the largest scoring advantage.

## Official Documents
[Section 0 - Introduction](https://web.archive.org/web/20060622211102/http://www2.usfirst.org/2006comp/Manual/0-Introduction.pdf "https://web.archive.org/web/20060622211102/http://www2.usfirst.org/2006comp/Manual/0-Introduction.pdf")  
[Section 1 - Communication](https://web.archive.org/web/20060622212326/http://www2.usfirst.org/2006comp/Manual/1-Communication_RevD.pdf "https://web.archive.org/web/20060622212326/http://www2.usfirst.org/2006comp/Manual/1-Communication_RevD.pdf")  
[Section 2 - Team Organization](https://web.archive.org/web/20060622210604/http://www2.usfirst.org/2006comp/Manual/2-Team_Org.pdf "https://web.archive.org/web/20060622210604/http://www2.usfirst.org/2006comp/Manual/2-Team_Org.pdf")  

### Section 3 - The Arena
[Section 3 - The Arena](https://web.archive.org/web/20060622211931/http://www2.usfirst.org/2006comp/Manual/3-The_Arena_Rev_B.pdf "https://web.archive.org/web/20060622211931/http://www2.usfirst.org/2006comp/Manual/3-The_Arena_Rev_B.pdf")  
[2006 _FIRST_ Robotics Competition Field Layout and Marking](https://web.archive.org/web/20130403174034/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Layout_and_Marking_R3.pdf "https://web.archive.org/web/20130403174034/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Layout_and_Marking_R3.pdf")  
[2006 _FIRST_ Robotics Competition Advance Material List](https://web.archive.org/web/20061010041549/http://www2.usfirst.org/2006comp/AdvanceBuy_2006_r4.pdf "https://web.archive.org/web/20061010041549/http://www2.usfirst.org/2006comp/AdvanceBuy_2006_r4.pdf")  

#### Team Drawings
[2006 _FIRST_ Robotics Competition Game Team Field Elements Center Goal Sheet 1 of 3](https://web.archive.org/web/20060114082008/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL(1_of_3).pdf "https://web.archive.org/web/20060114082008/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL(1_of_3).pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Center Goal Sheet 2 of 3](https://web.archive.org/web/20160321094926/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL%282_of_3%29.pdf "https://web.archive.org/web/20160321094926/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL%282_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Center Goal Sheet 3 of 3](https://web.archive.org/web/20160321094916/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL%283_of_3%29.pdf "https://web.archive.org/web/20160321094916/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL%283_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Center Goal Chain Installation](https://web.archive.org/web/20160321094922/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL_CHAIN_INSTALLATION.pdf "https://web.archive.org/web/20160321094922/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CENTER_GOAL_CHAIN_INSTALLATION.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Corner Goal Sheet 1 of 3](https://web.archive.org/web/20160321094924/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CORNER_GOAL%281_of_3%29.pdf "https://web.archive.org/web/20160321094924/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CORNER_GOAL%281_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Corner Goal Sheet 2 of 3](https://web.archive.org/web/20160321094920/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CORNER_GOAL%282_of_3%29.pdf "https://web.archive.org/web/20160321094920/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CORNER_GOAL%282_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Corner Goal Sheet 3 of 3](https://web.archive.org/web/20160321094926/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CORNER_GOAL%283_of_3%29.pdf "https://web.archive.org/web/20160321094926/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_CORNER_GOAL%283_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Platform Sheet 1 of 3](https://web.archive.org/web/20160321094922/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_PLATFORM%281_of_3%29R1.pdf "https://web.archive.org/web/20160321094922/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_PLATFORM%281_of_3%29R1.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Platform Sheet 2 of 3](https://web.archive.org/web/20160321094918/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_PLATFORM%282_of_3%29.pdf "https://web.archive.org/web/20160321094918/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_PLATFORM%282_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Platform Sheet 3 of 3](https://web.archive.org/web/20070317032850/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_PLATFORM(3_of_3).pdf "https://web.archive.org/web/20070317032850/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_PLATFORM(3_of_3).pdf")  
[2006 _FIRST_ Robotics Competition Game Team Field Elements Vision Target](https://web.archive.org/web/20060114075508/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_VISION_TARGET.pdf "https://web.archive.org/web/20060114075508/http://www2.usfirst.org/2006comp/Drawings/2006_TFE_VISION_TARGET.pdf")

#### Official _FIRST_ Drawings
[2006 _FIRST_ Robotics Competition Game Official Field Elements Center Goal Sheet 1 of 3](https://web.archive.org/web/20111111183330/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Center_Goal_Sheet_(1_of_3)R1.pdf "https://web.archive.org/web/20111111183330/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Center_Goal_Sheet_(1_of_3)R1.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Center Goal Sheet 2 of 3](https://web.archive.org/web/20160321094956/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Center_Goal_Sheet_%282_of_3%29R1.pdf "https://web.archive.org/web/20160321094956/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Center_Goal_Sheet_%282_of_3%29R1.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Center Goal Sheet 3 of 3](https://web.archive.org/web/20060114082504/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Center_Goal_Sheet_(3_of_3)R1.pdf "https://web.archive.org/web/20060114082504/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Center_Goal_Sheet_(3_of_3)R1.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Center Goal Chain Installation](https://web.archive.org/web/20160321095014/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_CENTER_GOAL_CHAIN_INSTALLATION.pdf "https://web.archive.org/web/20160321095014/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_CENTER_GOAL_CHAIN_INSTALLATION.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Corner Goal Sheet 1 of 3](https://web.archive.org/web/20070117004853/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Corner_Goal_Sheet(1_of_3).pdf "https://web.archive.org/web/20070117004853/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Corner_Goal_Sheet(1_of_3).pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Corner Goal Sheet 2 of 3](https://web.archive.org/web/20160321095010/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Corner_Goal_Sheet%282_of_3%29.pdf "https://web.archive.org/web/20160321095010/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Corner_Goal_Sheet%282_of_3%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Corner Goal Sheet 3 of 3](https://web.archive.org/web/20160321095003/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Corner_Goal_Sheet%283_of_3%29R3.pdf "https://web.archive.org/web/20160321095003/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Corner_Goal_Sheet%283_of_3%29R3.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Ball Corral](https://web.archive.org/web/20160321094954/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Ball_Corral.pdf "https://web.archive.org/web/20160321094954/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Ball_Corral.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Platform Sheet 1 of 4](https://web.archive.org/web/20070117004538/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet(1_of_4).pdf "https://web.archive.org/web/20070117004538/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet(1_of_4).pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Platform Sheet 2 of 4](https://web.archive.org/web/20070117004616/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet(2_of_4).pdf "https://web.archive.org/web/20070117004616/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet(2_of_4).pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Platform Sheet 3 of 4](https://web.archive.org/web/20070117004658/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet(3_of_4).pdf "https://web.archive.org/web/20070117004658/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet(3_of_4).pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Platform Sheet 4 of 4](https://web.archive.org/web/20160321095010/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet%284_of_4%29.pdf "https://web.archive.org/web/20160321095010/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Platform_Sheet%284_of_4%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Vision Target Sheet 1 of 2](https://web.archive.org/web/20160321094959/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Vision_Target_Sheet%281_of_2%29.pdf "https://web.archive.org/web/20160321094959/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Vision_Target_Sheet%281_of_2%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Vision Target Sheet 2 of 2](https://web.archive.org/web/20160321095006/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Vision_Target_Sheet%282_of_2%29.pdf "https://web.archive.org/web/20160321095006/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Vision_Target_Sheet%282_of_2%29.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Corner Support Assembly](https://web.archive.org/web/20160321094955/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Corner_Support_Assy.pdf "https://web.archive.org/web/20160321094955/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Corner_Support_Assy.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Corner Support Fabrication](https://web.archive.org/web/20160321095015/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Corner_Support_Fab.pdf "https://web.archive.org/web/20160321095015/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Corner_Support_Fab.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements End Panel Assembly](https://web.archive.org/web/20060114075440/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Panel_Assy.pdf "https://web.archive.org/web/20060114075440/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Panel_Assy.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements End Panel Fabrication](https://web.archive.org/web/20060114065919/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Panel_Fab.pdf "https://web.archive.org/web/20060114065919/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Panel_Fab.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements End Support Assembly](https://web.archive.org/web/20160321095001/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Support_Assy.pdf "https://web.archive.org/web/20160321095001/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Support_Assy.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements End Support Fabrication](https://web.archive.org/web/20160321095004/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Support_Fab.pdf "https://web.archive.org/web/20160321095004/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_End_Support_Fab.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Field Gate Fabrication and Assembly](https://web.archive.org/web/20160321094958/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Gate_Fab_&_Assy.pdf "https://web.archive.org/web/20160321094958/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Gate_Fab_&_Assy.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Hinge Fabrication](https://web.archive.org/web/20160321095009/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Hinge_Fab.pdf "https://web.archive.org/web/20160321095009/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Hinge_Fab.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Lexan Fabrication](https://web.archive.org/web/20160321094947/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Lexan_Fab.pdf "https://web.archive.org/web/20160321094947/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Lexan_Fab.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Outrigger Fabrication and Assembly](https://web.archive.org/web/20160321094946/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Outrigger_Fab_&_Assy.pdf "https://web.archive.org/web/20160321094946/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Outrigger_Fab_&_Assy.pdf")  
[2006 _FIRST_ Robotics Competition Game Official Field Elements Rail Fabrication and Assembly](https://web.archive.org/web/20160321094952/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Rail_Fab_&_Assy.pdf "https://web.archive.org/web/20160321094952/http://www2.usfirst.org/2006comp/Drawings/2006_FRC_Field_Rail_Fab_&_Assy.pdf")  
2006 _FIRST_ Robotics Competition Game Official Field Elements Top Rail Fabrication and Assembly (File not found as of 3/10/17)  
2006 _FIRST_ Robotics Competition Game Official Field Elements Weight Fabrication and Assembly (File not found as of 3/10/17)  
  
[Section 4 - The Game](https://web.archive.org/web/20061010041919/http://www2.usfirst.org/2006comp/Manual/4-The_Game,_Rev_F.pdf "https://web.archive.org/web/20061010041919/http://www2.usfirst.org/2006comp/Manual/4-The_Game,_Rev_F.pdf")  

### Section 5 - The Robot (includes the Kit of Parts)
[Section 5 - The Robot (includes the Kit of Parts)](https://web.archive.org/web/20060902090301/http://www2.usfirst.org/2006comp/Manual/5-The_Robot_Rev_F.pdf "https://web.archive.org/web/20060902090301/http://www2.usfirst.org/2006comp/Manual/5-The_Robot_Rev_F.pdf")

#### Drawings
[2006 Robot Power Distribution Diagram (.pdf)](https://web.archive.org/web/20060206032500/http://www2.usfirst.org/2006comp/Drawings/2006_ROBOT_POWER_DISTRIBUTION.pdf "https://web.archive.org/web/20060206032500/http://www2.usfirst.org/2006comp/Drawings/2006_ROBOT_POWER_DISTRIBUTION.pdf")  
[2006 Robot Power Distribution Diagram (.dxf)](https://web.archive.org/web/20060621162501/http://www2.usfirst.org/2006comp/Drawings/2006_ROBOT_POWER_DISTRIBUTION.dxf "https://web.archive.org/web/20060621162501/http://www2.usfirst.org/2006comp/Drawings/2006_ROBOT_POWER_DISTRIBUTION.dxf")

#### Other Important Documents
[2006 _FIRST_ Robotics Inspection Manual](https://web.archive.org/web/20151123083001/http://www2.usfirst.org/2006comp/other/2006_Robot_Inspection_Manual-narrated_rev_D.pdf "https://web.archive.org/web/20151123083001/http://www2.usfirst.org/2006comp/other/2006_Robot_Inspection_Manual-narrated_rev_D.pdf")  
2006 _FIRST_ Robotics Inspection Checklist (File not found as of 3/10/17)  
[2006 _FIRST_ Welcome to Robotics Inspection](https://web.archive.org/web/20060902140927/http://www2.usfirst.org/2006comp/other/2006_Welcome_to_Robot_Inspection-rev_D.pdf "https://web.archive.org/web/20060902140927/http://www2.usfirst.org/2006comp/other/2006_Welcome_to_Robot_Inspection-rev_D.pdf")  
[2006 _FIRST_ Robotics Inspection Possible Station Layout](https://web.archive.org/web/20160321094935/http://www2.usfirst.org/2006comp/other/2006_Robot_Inspection-possible_station_layout1.pdf "https://web.archive.org/web/20160321094935/http://www2.usfirst.org/2006comp/other/2006_Robot_Inspection-possible_station_layout1.pdf")  
[2006 _FIRST_ Robotics Inspection Scale](https://web.archive.org/web/20160321094931/http://www2.usfirst.org/2006comp/other/Robot_Inspection_scale1.pdf "https://web.archive.org/web/20160321094931/http://www2.usfirst.org/2006comp/other/Robot_Inspection_scale1.pdf")  
[2006 _FIRST_ Robotics Inspection Sizing Box](https://web.archive.org/web/20160321094944/http://www2.usfirst.org/2006comp/other/Robot_Inspection_SIZING_BOX1.pdf "https://web.archive.org/web/20160321094944/http://www2.usfirst.org/2006comp/other/Robot_Inspection_SIZING_BOX1.pdf")  
[Inspection - Conference Call Minutes 03-06-06](https://web.archive.org/web/20160321094934/http://www2.usfirst.org/2006comp/other/Inspection-Conference_Call_Minutes_03-06-06.pdf "https://web.archive.org/web/20160321094934/http://www2.usfirst.org/2006comp/other/Inspection-Conference_Call_Minutes_03-06-06.pdf")  

#### 2006 _FIRST_ Robotics Competition Specification Sheets
[Allegro Gear Tooth Sensor](https://web.archive.org/web/20060110165853/http://www2.usfirst.org/2006comp/Specs/Allegro_Microsystems_Gear_tooth_Sensor.pdf "https://web.archive.org/web/20060110165853/http://www2.usfirst.org/2006comp/Specs/Allegro_Microsystems_Gear_tooth_Sensor.pdf")  
[Allen Bradley Photo Detector Sensor](https://web.archive.org/web/20061231172954/http://www2.usfirst.org/2006comp/Specs/Allen_Bradley_photodetector.pdf "https://web.archive.org/web/20061231172954/http://www2.usfirst.org/2006comp/Specs/Allen_Bradley_photodetector.pdf")  
[Analog Devices Ultracompact Dual-Axis Accelerometer](https://web.archive.org/web/20140122012040/http://www2.usfirst.org/2006comp/Specs/Analog_Devices_Ultracompact_Dual-Axis_Accelerometer.pdf "https://web.archive.org/web/20140122012040/http://www2.usfirst.org/2006comp/Specs/Analog_Devices_Ultracompact_Dual-Axis_Accelerometer.pdf")  
[Analog Devices Yaw Rate Gyro Sensor](https://web.archive.org/web/20061231173025/http://www2.usfirst.org/2006comp/Specs/Analog_Devices_Yaw_Rate_Gyro.pdf "https://web.archive.org/web/20061231173025/http://www2.usfirst.org/2006comp/Specs/Analog_Devices_Yaw_Rate_Gyro.pdf")  
[CIM](https://web.archive.org/web/20070203122606/http://www2.usfirst.org/2005comp/Specs/CIM.pdf "https://web.archive.org/web/20070203122606/http://www2.usfirst.org/2005comp/Specs/CIM.pdf")  
[CIM Motor FR801-005](https://web.archive.org/web/20061214211314/http://www2.usfirst.org/2006comp/Specs/CIM_Motor_FR801-005.pdf "https://web.archive.org/web/20061214211314/http://www2.usfirst.org/2006comp/Specs/CIM_Motor_FR801-005.pdf")  
[Clippard Volume Tank](https://web.archive.org/web/20061231173008/http://www2.usfirst.org/2005comp/Specs/Clippard_Volume_tank.pdf "https://web.archive.org/web/20061231173008/http://www2.usfirst.org/2005comp/Specs/Clippard_Volume_tank.pdf")  
[Denso Window Motor](https://web.archive.org/web/20061214211629/http://www2.usfirst.org/2006comp/Specs/Denso_Motor.pdf "https://web.archive.org/web/20061214211629/http://www2.usfirst.org/2006comp/Specs/Denso_Motor.pdf")  
[Exide 12V Battery](https://web.archive.org/web/20050204230216/http://www2.usfirst.org/2005comp/Specs/batex.pdf "https://web.archive.org/web/20050204230216/http://www2.usfirst.org/2005comp/Specs/batex.pdf")  
[Festo Valve](https://web.archive.org/web/20050204232740/http://www2.usfirst.org/2005comp/Specs/Festo1.pdf "https://web.archive.org/web/20050204232740/http://www2.usfirst.org/2005comp/Specs/Festo1.pdf")  
[Fisher-Price Motor 9003](https://web.archive.org/web/20061214211551/http://www2.usfirst.org/2006comp/Specs/Fisher_Price_Motor_FP9003.pdf "https://web.archive.org/web/20061214211551/http://www2.usfirst.org/2006comp/Specs/Fisher_Price_Motor_FP9003.pdf")  
[Fisher-Price Motor 9012](https://web.archive.org/web/20061214211552/http://www2.usfirst.org/2006comp/Specs/Fisher_Price_Motor_FP9012.pdf "https://web.archive.org/web/20061214211552/http://www2.usfirst.org/2006comp/Specs/Fisher_Price_Motor_FP9012.pdf")  
[Globe Motor](https://web.archive.org/web/20061231173020/http://www2.usfirst.org/2005comp/Specs/Globe_Motor.pdf "https://web.archive.org/web/20061231173020/http://www2.usfirst.org/2005comp/Specs/Globe_Motor.pdf")  
[Lord Vibration Isolators](https://web.archive.org/web/20050204224157/http://www2.usfirst.org/2005comp/Specs/lord1.pdf "https://web.archive.org/web/20050204224157/http://www2.usfirst.org/2005comp/Specs/lord1.pdf")  
[Mabuchi Motor](https://web.archive.org/web/20061214211644/http://www2.usfirst.org/2006comp/Specs/Mabuchi_Motor.pdf "https://web.archive.org/web/20061214211644/http://www2.usfirst.org/2006comp/Specs/Mabuchi_Motor.pdf")  
[Midtronics Battery Charger](https://web.archive.org/web/20140122011922/http://www2.usfirst.org/2006comp/Specs/Midtronics_battery_charger.pdf "https://web.archive.org/web/20140122011922/http://www2.usfirst.org/2006comp/Specs/Midtronics_battery_charger.pdf")  
[Norgren Gauge](https://web.archive.org/web/20060428073643/http://www2.usfirst.org/2005comp/Specs/Norgau.pdf "https://web.archive.org/web/20060428073643/http://www2.usfirst.org/2005comp/Specs/Norgau.pdf")  
[Norgren Main Regulator](https://web.archive.org/web/20050204233438/http://www2.usfirst.org/2005comp/Specs/Noreg.pdf "https://web.archive.org/web/20050204233438/http://www2.usfirst.org/2005comp/Specs/Noreg.pdf")  
[Papst Fan, Large](https://web.archive.org/web/20050204231654/http://www2.usfirst.org/2005comp/Specs/fan1.pdf "https://web.archive.org/web/20050204231654/http://www2.usfirst.org/2005comp/Specs/fan1.pdf")  
[Papst Fan, Small](https://web.archive.org/web/20050204222848/http://www2.usfirst.org/2005comp/Specs/fan2.pdf "https://web.archive.org/web/20050204222848/http://www2.usfirst.org/2005comp/Specs/fan2.pdf")  
[Rexroth Value](https://web.archive.org/web/20061231173051/http://www2.usfirst.org/2006comp/Specs/Rexroth.pdf "https://web.archive.org/web/20061231173051/http://www2.usfirst.org/2006comp/Specs/Rexroth.pdf")  
[Skyway 8" Wheel](https://web.archive.org/web/20050204224033/http://www2.usfirst.org/2005comp/Specs/skyway.pdf "https://web.archive.org/web/20050204224033/http://www2.usfirst.org/2005comp/Specs/skyway.pdf")  
[SMC Double Solenoid](https://web.archive.org/web/20050204222202/http://www2.usfirst.org/2005comp/Specs/SY3000.pdf "https://web.archive.org/web/20050204222202/http://www2.usfirst.org/2005comp/Specs/SY3000.pdf")  
[SMC Flow Control Valve](https://web.archive.org/web/20050204234000/http://www2.usfirst.org/2005comp/Specs/Floctl.pdf "https://web.archive.org/web/20050204234000/http://www2.usfirst.org/2005comp/Specs/Floctl.pdf")  
SMC Fittings (File not found as of 3/10/17)  
[Snap Action Circuit Breaker](https://web.archive.org/web/20061231173051/http://www2.usfirst.org/2006comp/Specs/Snap_Action_CBs.pdf "https://web.archive.org/web/20061231173051/http://www2.usfirst.org/2006comp/Specs/Snap_Action_CBs.pdf")  
[Wika Gauges](https://web.archive.org/web/20050204225629/http://www2.usfirst.org/2005comp/Specs/wika1.pdf "https://web.archive.org/web/20050204225629/http://www2.usfirst.org/2005comp/Specs/wika1.pdf")  
  
[Kit of Parts Checklist and Photo Album](https://web.archive.org/web/20061214212039/http://www2.usfirst.org/2006comp/other/KOP_CheckList_&_Photos-Rev_A.pdf "https://web.archive.org/web/20061214212039/http://www2.usfirst.org/2006comp/other/KOP_CheckList_&_Photos-Rev_A.pdf")  
[Additional Material List](https://web.archive.org/web/20061222141308/http://www2.usfirst.org/2006comp/other/Additional_Material.pdf "https://web.archive.org/web/20061222141308/http://www2.usfirst.org/2006comp/other/Additional_Material.pdf")  
[2006 _FIRST_ Pneumatics Manual](https://web.archive.org/web/20061222141520/http://www2.usfirst.org/2006comp/other/2006_FIRST_Pneumatics_Manual.pdf "https://web.archive.org/web/20061222141520/http://www2.usfirst.org/2006comp/other/2006_FIRST_Pneumatics_Manual.pdf")  
[2006 CMUCam2 Workbook](https://web.archive.org/web/20060811015003/http://www2.usfirst.org/2006comp/other/2006_CMUCam2_Workbook-Rev_B.pdf "https://web.archive.org/web/20060811015003/http://www2.usfirst.org/2006comp/other/2006_CMUCam2_Workbook-Rev_B.pdf")  
[Batteries Plus Order Form](https://web.archive.org/web/20070710194643/http://www2.usfirst.org/2006comp/other/Battery_Order_Form_ES18-12.pdf "https://web.archive.org/web/20070710194643/http://www2.usfirst.org/2006comp/other/Battery_Order_Form_ES18-12.pdf")  
[2006 Sensor Basic Operation](https://web.archive.org/web/20061231172835/http://www2.usfirst.org/2006comp/other/2006_Sensor_Basic_Operation.pdf "https://web.archive.org/web/20061231172835/http://www2.usfirst.org/2006comp/other/2006_Sensor_Basic_Operation.pdf")  
[2006 _FIRST_ Guidelines, Tips & Good Practices](https://web.archive.org/web/20061220194710/http://www2.usfirst.org/2006comp/other/FIRST_Guidelines,_Tips,_&_Good_Practices_Rev_D.pdf "https://web.archive.org/web/20061220194710/http://www2.usfirst.org/2006comp/other/FIRST_Guidelines,_Tips,_&_Good_Practices_Rev_D.pdf")  
[2006 _FIRST_ Robotics Competition Software Overview](https://web.archive.org/web/20060221031749/http://www.usfirst.org/robotics/2006/2006frcsoftwareoverview.htm "https://web.archive.org/web/20060221031749/http://www.usfirst.org/robotics/2006/2006frcsoftwareoverview.htm")  
  
[Section 6 - Robot Transportation](https://web.archive.org/web/20060622212817/http://www2.usfirst.org/2006comp/Manual/6-Robot_Transportation_Rev_C.pdf "https://web.archive.org/web/20060622212817/http://www2.usfirst.org/2006comp/Manual/6-Robot_Transportation_Rev_C.pdf")  
[Section 7 - At the Event](https://web.archive.org/web/20060622212451/http://www2.usfirst.org/2006comp/Manual/7-At_the_Events_Rev_C.pdf "https://web.archive.org/web/20060622212451/http://www2.usfirst.org/2006comp/Manual/7-At_the_Events_Rev_C.pdf")  
[Section 8 - The Tournament](https://web.archive.org/web/20060205044337/http://www2.usfirst.org/2006comp/Manual/8-The_Tournament.pdf "https://web.archive.org/web/20060205044337/http://www2.usfirst.org/2006comp/Manual/8-The_Tournament.pdf")  
[Section 9 - The Awards](https://web.archive.org/web/20060622210538/http://www2.usfirst.org/2006comp/Manual/9-Awards_RevD.pdf "https://web.archive.org/web/20060622210538/http://www2.usfirst.org/2006comp/Manual/9-Awards_RevD.pdf")  
[Section 10 - Get Published](https://web.archive.org/web/20060205035141/http://www2.usfirst.org/2006comp/Manual/10-Publisher.pdf "https://web.archive.org/web/20060205035141/http://www2.usfirst.org/2006comp/Manual/10-Publisher.pdf")  

### Team Updates
Team Update #1 (File not found as of 3/10/17)  
Team Update #2 (File not found as of 3/10/17)  
Team Update #3 (File not found as of 3/10/17)  
[Team Update #4](https://web.archive.org/web/20070710194544/http://www2.usfirst.org/2006comp/Updates/Team_Update_4_Jan-27-06.pdf "https://web.archive.org/web/20070710194544/http://www2.usfirst.org/2006comp/Updates/Team_Update_4_Jan-27-06.pdf")  
Team Update #5 (File not found as of 3/10/17)  
Team Update #6 (File not found as of 3/10/17)  
[Team Update #7](https://web.archive.org/web/20070330070501/http://www2.usfirst.org/2006comp/Updates/Team_Update_7_Feb-8-06.pdf "https://web.archive.org/web/20070330070501/http://www2.usfirst.org/2006comp/Updates/Team_Update_7_Feb-8-06.pdf")  
Team Update #8 (File not found as of 3/10/17)  
Team Update #9 (File not found as of 3/10/17)  
[Team Update #10](https://web.archive.org/web/20151103222150/http://www2.usfirst.org/2006comp/Updates/Team_Update_10_Feb-17-06.pdf "https://web.archive.org/web/20151103222150/http://www2.usfirst.org/2006comp/Updates/Team_Update_10_Feb-17-06.pdf")

