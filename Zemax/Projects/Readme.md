# Microscope Objective Lens Design

This repository contains a microscope objective lens design created in Zemax OpticStudio. The design is inspired by the Ansys webinar "[Designing a Microscope Objective with OpticStudio](https://optics.ansys.com/hc/en-us/articles/42661787388947-Designing-a-microscope-objective-with-OpticStudio-webinar)".

## Specifications

The design meets the following key performance specifications:
*   **Effective Focal Length (EFL):** 3.67 mm
*   **Entrance Pupil Diameter (EPD):** 6.98 mm
*   **Total Track Length:** 11.56 mm (very compact)
*   **Paraxial Image Height:** 0.169 mm
*   **Wavelength:** Visible spectrum (F, d, C - 486.1nm, 587.6nm, 656.3nm)

## Design Overview

This is a multi-element objective lens, a critical component in microscopy, requiring excellent correction for optical aberrations to produce a clear, sharp image.

**Key Features:**
*   **High Numerical Aperture (NA):** The fast F/# implies a high NA, which is essential for high resolution and light-gathering capability.
*   **Achromatic Design:** Corrected for chromatic aberration across the visible spectrum.
*   **Compact Form Factor:** The entire optical system is designed within a very short physical length.

## File: `MicroscopeObjective_tolerence_ready.zmx`

This Zemax file represents the final, optimized design that is prepared for a full tolerance analysis.


## ℹ️ Important Note on Student Version Limitation

**This design has not undergone a full tolerance analysis.**

The Zemax OpticStudio Student Version has a limitation that prevents running the Monte Carlo tolerance analysis. Therefore, while the file is fully set up and "ready" for this process, the analysis itself could not be performed.

In a professional setting, the next steps would be:
1.  Defining tolerances for each parameter (e.g., lens thickness ±0.05 mm, radius curvature ±0.01 mm).
2.  Running a Monte Carlo analysis to simulate hundreds of randomly assembled systems.
3.  Analyzing the results to see if the design is robust enough for manufacture or if certain tolerances need to be tightened.

## How to Use

1.  Open the `.zmx` file in Zemax OpticStudio (v20.2+ recommended).
2.  Analyze the performance using features like the Layout, MTF Chart, Spot Diagram, and Field Curvature/Distortion plots.
3.  **Full Version Users:** You can proceed to the Tolerance tab to define compensators and run a Monte Carlo analysis to test the design's manufacturability.

## Learning Resources

The design principles and workflow for this objective are based on the excellent webinar by Ansys:
*   **[Webinar: Designing a Microscope Objective with OpticStudio](https://optics.ansys.com/hc/en-us/articles/42661787388947-Designing-a-microscope-objective-with-OpticStudio-webinar)**
*   This webinar provides a step-by-step guide on how to set up, optimize, and analyze such a complex system.

## Related Projects

For more fundamental optical design examples, please see the main directory of this repository: [Basic Optical Design Templates](https://github.com/KBG0603/Optical-design/tree/main/Zemax/Basic-templates).

## License

This project is shared for educational and learning purposes.
