# Forensic Reverse-Projection Pipeline
## Blender + OpenCV PnP Forensic Workflow
**Robert Bryan · October 2025**

## Overview
This document presents a validated forensic reverse-projection pipeline implementing Perspective-n-Point (PnP) camera pose estimation using Blender and OpenCV. This is one of the first openly documented, reproducible implementations of these principles using publicly available tools for forensic reconstruction purposes.

Commercial forensic software such as iNPUT-ACE (Axon Investigate) and FARO/ARAS 360 employ similar PnP-based camera models. Their calibration workflows are proprietary. This work provides a transparent, auditable alternative.

## Validation Results
- Closed-loop validation: **1.04px RMS** reprojection error across 32 reference points
- Open-loop validation: **5.16px RMS** reprojection error under real-world conditions with unknown camera intrinsics

Corresponding spatial margins of error:
- Closed-loop: approximately ±1.4cm at 120m
- Open-loop: approximately ±7cm

## Tools Used
- [Blender](https://www.blender.org)
- [OpenCV](https://opencv.org)
- [camera-pnpoint addon](https://github.com/RT-studios/camera-pnpoint)

## Documentation
See Reverse_Projection_Pipeline.pdf for full methodology, figures, and validation analysis.

## Related Forensic Software (Referenced for Context)
- iNPUT-ACE / Axon Investigate — https://www.axon.com/products/axon-investigate
- ARAS 360 — https://aras360.com
- PhotoModeler — https://www.photomodeler.com

## Author
Robert Bryan — Forensic Visualization & Reconstruction · rlbryansr@gmail.com
October 2025

## License
MIT License — open source, free to use, modify, and build upon with attribution.
