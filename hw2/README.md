# HW2 — Sumo Robot Design and Implementation

Team: **Team 8**

## Members
- Chung-Yu Chang (張仲瑜): Main graphical programming, testing
- Yuan-Rui Xu (許元瑞): Assistant graphical programming, robot assembly
- Bo-Yun Lai (賴博允): Robot assembly, design
- Zi-Yang Zhou (周子揚): Robot assembly, testing
- Yao-Ting Tsai (蔡耀霆): Robot assembly, testing

## Introduction
The primary goal of this project was to design a sumo robot (both hardware and software algorithm) capable of pushing or flipping opponents out of the arena. Our design features a low chassis for center-of-gravity stability and a front-mounted "plow" (incisor) to lift or push the enemy.

## Core Strategy
Our winning strategy revolves around speed and positioning:
- Early entry: Sprint to the arena first, then block the opponent’s entry point for 15 seconds to force a timeout.
- Combat Logic: If the opponent enters: Retreat to the center, rotate to scan, then launch a full-speed push.

## Implementation Details
- Platform: Graphical programming (Spike Prime / EV3) for motion and sensing.
- Navigation: Line-following on white/black with an acceleration profile tuned for sharp turns.
- Boundary safety: Color sensor has top priority; detects the red boundary and immediately reverses to stay inside.
- Detection & attack: Distance sensor locks targets within ~40 cm, then triggers a fast rotation-and-push maneuver.

## Demonstration
- Click [HW2_team8.pdf](HW2_team8.pdf) for the detailed report.
- A video demonstration is available [here](https://drive.google.com/drive/folders/1C6o8mXlgtbcCujPbG6WgAqitYx1EgM17).