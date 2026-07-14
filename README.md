# Passive Solar Tracking System

A fully passive, single-axis solar tracker that follows the sun using **paraffin wax phase-change actuation** — no motors, no sensors, no electricity.

ME 325 — Third Year Engineering Project 
---

## Demo

[Watch the mechanism in action (YouTube, unlisted)](https://youtu.be/zYTDFJzssF4)

---

## Overview

Most solar trackers rely on motors and control electronics to reorient a panel throughout the day — effective, but costly to install and maintain. This project takes a different approach: **thermal actuation**.

A parabolic concentrator focuses solar radiation onto a receiver tube filled with paraffin wax. As the wax heats past its melting point, it undergoes a solid-to-liquid phase change and expands. This expansion drives a piston, which — through a mechanical linkage — rotates the solar panel to track the sun's path across the sky, entirely without external power.

### Objectives

**Main objective**
Design and develop a fully passive single-axis solar tracker using paraffin wax expansion.

**Specific objectives**
- Track the sun for 8 hours
- Zero electricity consumption
- Maximum tracking lag < 8°
- Low maintenance
- Suitable for Sri Lankan climate conditions
- Affordable fabrication

---

## How It Works

```
Solar Radiation → Parabolic Concentrator → Receiver Tube
       → Paraffin Wax Heating → Phase Change → Volume Increase
       → Piston Motion → Mechanical Linkage → Solar Panel Rotation
```

As the wax melts and expands, hydraulic pressure pushes the piston outward. This linear motion is converted into rotational motion that tilts the panel toward the sun. As ambient conditions cool later in the day, the wax contracts and the mechanism resets — ready to track again the next morning.

---

## Design Rationale: Paraffin Wax vs. Refrigerant System

Two thermal actuation approaches were evaluated during concept selection. Paraffin wax was chosen for its safety, simplicity, and low cost.

| Criterion | Refrigerant System | Paraffin Wax System |
|---|---|---|
| Safety | High pressure fluid | Low pressure operation |
| Leakage risk | High | Very low |
| Manufacturing complexity | High | Simple |
| Sealing requirements | Critical | Moderate |
| Maintenance | High | Low |
| Cost | Higher | Lower |
| Availability | Requires procurement | Easily available |

---

## Engineering Analysis

Key design parameters derived from thermal, phase-change, and mechanical modeling:

| Parameter | Value |
|---|---|
| Aperture area | 0.11935 m² |
| Wax mass | 0.27 kg |
| Energy to reach melting point (30°C → 58°C) | 18,900 J |
| Effective wax volume change | 4.5 × 10⁻⁵ m³ |
| Maximum piston stroke | 35.8 mm |
| Required mechanical amplification | 2.79°/mm |

### Simulated Performance

| Metric | Result |
|---|---|
| Wax temperature range | 30°C → 65°C |
| Full melt achieved | By 3 PM |
| Panel rotation | 0° → 100° |
| Maximum tracking lag | 5–7° |
| Tracking range | ≈ 120° |

Simulation (Excel/MATLAB) confirmed the design meets the target lag of under 8° across the tracking window, with the mechanism reaching full wax melt in the early afternoon and maintaining close solar alignment for the remainder of the day.

---

## Project Status

| Milestone | Status |
|---|---|
| Literature Review & Patent Analysis | ✅ Complete |
| Concept Selection & Design Methodology | ✅ Complete |
| Mathematical Modeling | ✅ Complete |
| CAD Design & System Architecture | 🔶 90% — minor refinements ongoing |
| Excel/MATLAB Simulation | 🔶 85% — tracking angle and lag analysis complete |
| Prototype Fabrication Planning | 🔶 70% — material selection and drawings in progress |

---

## Presentation

[View full project presentation](docs/presentation.pdf)

---
