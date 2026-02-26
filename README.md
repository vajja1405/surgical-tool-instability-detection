# Surgical Tool Instability Prediction using Deep Learning

Graduate Research – University of Missouri–Kansas City  
Advisor: Prof. Cheng Han  
Status: Ongoing (Jan 2026 – Present)

## Overview

This project develops a deep learning-based video analysis framework to quantify surgical tool motion instability using robotic surgery videos (JIGSAWS suturing task).

The system integrates:

- YOLOv8-based tool tip detection
- Multi-frame tracking
- Trajectory-based kinematic modeling (velocity, acceleration, jerk)
- Quantitative instability metrics for motion smoothness assessment

## Motivation

Surgical precision directly impacts patient outcomes. This research aims to develop objective, data-driven motion smoothness metrics that can:

- Detect micro-instabilities
- Support surgical skill assessment
- Enable automated feedback systems

## Methodology

1. Tool Detection
   - YOLOv8 fine-tuned on JIGSAWS frames
   - Tool-tip localization per frame

2. Tracking
   - Frame-to-frame trajectory reconstruction

3. Kinematic Modeling
   - Velocity: first derivative of position
   - Acceleration: second derivative
   - Jerk: third derivative

4. Instability Indicators
   - High jerk variance
   - Irregular acceleration spikes
   - Motion smoothness index

## Tech Stack

- Python
- PyTorch
- YOLOv8 (Ultralytics)
- NumPy
- OpenCV
- Matplotlib

## Future Work

- Real-time inference
- Multi-tool instability detection
- Surgeon skill classification
