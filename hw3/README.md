# HW3 — Robot Road Test

Team: **Team 8**

## Members
- Chung-Yu Chang (張仲瑜): Main graphical programming, testing
- Yuan-Rui Xu (許元瑞): Assistant graphical programming, robot assembly
- Bo-Yun Lai (賴博允): Robot assembly, design
- Zi-Yang Zhou (周子揚): Robot assembly, testing
- Yao-Ting Tsai (蔡耀霆): Robot assembly, testing

## Introduction
The objective of this project was to design a robot (both hardware and software algorithm) capable of successfully navigating two distinct road test tracks (Demo 1 and Demo 2). The test involves mastering five specific maneuvers: parallel parking, reverse parking, S-curve navigation, straight-line driving, and general turns.

## Core Strategy
Our design focused on minimalism and stability:
- Compact body: Keep the chassis as small as possible to reduce physical variance and avoid accessory-induced instability.
- Simplified mechanics: Favor a robust, minimal build so repeated runs behave consistently.

## Implementation Details
- Approach: Graphical programming plus iterative trial-and-error tuning.
- Terrain-specific logic: Coefficients per maneuver were derived through repeated testing.
- Inertia management: Inserted pauses between continuous turns to cancel residual inertia; slower overall but more stable.
- Controlled speed: Lower motor speeds to keep wheel friction high for precise stops and turns.
- Reality vs. logic: Entering and exiting an S-curve cannot be simple mirrors because physical conditions differ.
- Empirical adjustment: Real-world factors demand iterative tuning beyond purely logical planning.

## Demonstration
- Click [HW3_team8.pdf](HW3_team8.pdf) for the detailed report.
- A video demonstration is available [here](https://drive.google.com/drive/folders/1nH__DUm7oth7qNoweb33b6GPI9hGtst9?usp=sharing).