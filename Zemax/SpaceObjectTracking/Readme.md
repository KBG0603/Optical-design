# Space Object Tracking with Refractive Optics

**Project for space surveillance applications**  
Author: Kaumudibikash Goswami  
Date: December 2025  

This repository contains a project on the optical design of a compact, wide-field lens system intended for detecting and tracking space objects (satellites, debris, etc.) from a small satellite payload.

## Project Goal
Design a **diffraction-limited** (as much as possible within constraints) refractive optical system that fits as many photons as possible (large aperture) while offering a **wide field of view** suitable for space surveillance.

### Main Constraints
- Maximum external volume: **90 mm × 90 mm × 180 mm**
- Entrance pupil must fit on the **90 × 90 mm** face
- Simple, manufacturable design (only spherical surfaces, no aspheres)

### Achieved Specifications
| Parameter                  | Value                     | Notes                                    |
|----------------------------|---------------------------|------------------------------------------|
| Entrance Pupil Diameter    | 60 mm                     | Fits inside 90 × 90 mm                   |
| Effective Focal Length     | 146.38 mm                 |                                          |
| f-number                   | f/2.44                    | Good light collection                    |
| Total Track Length         | 179 mm                    | < 180 mm limit                           |
| Back Focal Length          | 27.5 mm                   | Enough space for sensor + filter         |
| Field of View              | ±10° (20° full)           | Excellent for surveying large sky areas  |
| Image Circle Diameter      | ~51.6 mm (diagonal)       |                                          |

## Files in this Repository

- `Report.pdf` – Complete project report (LaTeX source also included)
- `Space_Application4.zmx` – **Ansys Zemax OpticStudio** file (Student Edition 2025 R1)

## Performance Summary

| Metric                     | Theoretical (Diffraction Limit) | Achieved (On-axis) | Achieved (10° off-axis) |
|----------------------------|---------------------------------|--------------------|-------------------------|
| Airy disk diameter         | ~3.5 µm                         | ~14.8 µm           | ~28.6 µm                |
| MTF cutoff frequency       | ~697 lp/mm                      | > 500 lp/mm        | ~400 lp/mm              |
| Angular resolution         | ~2.46 arcsec                    | ~10.4 arcsec (RMS) | worse at edge           |

The design is **not fully diffraction-limited** across the whole field (mainly limited by spherical aberration, field curvature, and some coma), but it is very respectable for an all-spherical, compact, fast (f/2.44) wide-field lens.

### Recommended Sensor
- Pixel size: **1.4–1.8 µm** (to properly sample the PSF even at the edge)
- Suitable sensors: Sony IMX455, IMX461, or similar high-resolution CMOS with small pixels

## Additional Notes for Satellite Use
The report includes a section on practical payload considerations:
- Athermalization
- Radiation-resistant glasses
- Stray light baffling
- Low-outgassing materials
- Launch vibration survival

These will be essential before flight.

## How to Open the Design
The optical design file (`Space_Application4.zmx`) can be opened with **Ansys Zemax OpticStudio** (any recent version, including the free Student Edition).

## License
This project is shared for educational and portfolio purposes. Feel free to use it as reference, but please give credit if you reuse parts of the design or report.

---

Thank you for checking out my space optics project!  
If you have questions, feel free to open an issue or contact me.
