# RoadEye

A front-camera perception project for vehicle and pedestrian detection, tracking, and training scene selection.

## Overview

RoadEye aims to detect and track vehicles and pedestrians in driving videos and select useful scenes for additional training. Occlusion handling will be explored depending on development progress.

## Planned Features

1. **Basic detection and tracking**
   - Detect vehicles and pedestrians using YOLO11n.
   - Track detected objects using ByteTrack.
   - Display and save detection results.

2. **Training scene selection**
   - Select review candidates using detection confidence.
   - Reduce near-duplicate scenes.
   - Incorporate detection discontinuities once tracking is available.
   - Compare selection methods under equal image-count and review-time budgets.

3. **Conditional occlusion handling**
   - Temporarily maintain estimated check areas using recent observations.
   - Evaluate selective re-detection after occlusion.
   - Proceed after the core features are complete, if time permits.

## Evaluation Plan

- **Detection:** Compare baseline training (B0) with brightness-augmented training (B1).
- **Scene selection:** Compare random, low-confidence, and proposed selection methods, retraining from the same baseline checkpoint.
- **Occlusion handling:** Compare re-detection delay, unnecessary attention indicators, and processing speed against the baseline.
- **System performance:** Measure processing speed and execution stability.

All performance targets in the project materials are provisional and have not yet been measured.

## Project Status

The project is currently in the planning and presentation preparation stage. Implementation has not started.

## Team

**RoadEye · Gachon University · SW Section 1, Team 3**

| Name | GitHub |
|---|---|
| 고근형 | [@kuenhyung](https://github.com/kuenhyung) |
| 김성원 | [@dkaaa01](https://github.com/dkaaa01) |
| 박시후 | [@Specialstr](https://github.com/Specialstr) |
| 신준하 | [@tjfdlvTkr](https://github.com/tjfdlvTkr) |

### Presentation Preparation Roles

| Members | Responsibilities |
|---|---|
| 김성원 · 신준하 | Prepare and deliver the presentation; record the presentation video and upload it to YouTube. |
| 박시후 · 고근형 | Research and organize the content; structure and produce the PowerPoint presentation. |

Development responsibilities will be assigned later.

## Project Documents

The project proposal and presentation materials will be maintained in the `docs/` directory.

## Intended Use

This project is intended for research and demonstration. It does not provide vehicle control or guarantee driving safety.
