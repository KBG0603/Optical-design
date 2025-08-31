# Basic Optical Design Templates (Zemax)

A collection of fundamental optical system designs made with Zemax OpticStudio. These projects are based on tutorials from Mark Nicholson's (CEO of Zemax) YouTube playlist, ["Design Optics Fast"](https://www.youtube.com/@DesignOpticsFast).

These files are useful for students and engineers who want to learn the principles of optical design and understand standard lens systems.

## Project Files

### 1. Simple Landscape Lens
*   **File:** `LandScape_Lens_F5.zmx`
*   **Description:** A basic single-lens system with the aperture stop (iris) behind the lens. This type of lens is often used in simple devices like motion detectors. It has many aberrations unless the aperture is very small. This example is an F/5 system.

### 2. Achromatic Doublet
*   **File:** `ColorCorrected.zmx`
*   **Description:** A single lens has color errors (chromatic aberration). This file shows how using two lenses together (a doublet) can correct this problem.

### 3. Corrected Landscape Lens
*   **File:** `ColorCorrected_LandScape_F5.zmx`
*   **Description:** This is an improved landscape lens. It uses a doublet instead of a single lens to control color errors better.

### 4. Landscape Lens with Front Iris
*   **File:** `LandScape_Lens_F5_drivatives.zmx`
*   **Description:** This is another version of the landscape lens, but the iris is placed in front of the lens. The performance is usually worse, but the whole system can be made smaller.

### 5. Petzval Landscape Lens
*   **File:** `LandScape_Lens_F5_drivatives3_petzvel.zmx`
*   **Description:** This design uses a Petzval arrangement. It is very good at correcting color errors and producing a flat image.

### 6. Cooke Triplet
*   **File:** `CookeTriplet.zmx`
*   **Description:** A classic three-lens design. It is very useful for systems that need a wide field of view because it corrects many aberrations well.

### 7. Double Gauss
*   **File:** `DoubleGauss.zmx`
*   **Description:** A famous design that is very good at controlling aberrations. It is often used in high-quality camera lenses.

### 8. Relay Lens Design (Step-by-Step)
This series shows how to add a relay lens to another optical system correctly.

*   **a) First Try:** `Relay.zmx`
    *   A simple start using a perfect (paraxial) lens. However, without matching the exit pupil of the primary lens system, the paraxial lens often turns out to be very large.

*   **b matching the Pupil:** `Relay_exit_pupilMatched.zmx`
    *   This file fixes the size problem by matching the relay lens's entrance pupil to the main system's exit pupil.

*   **c) Using Real Lenses:** `Relay_exit_pupilMatched_real_Lens.zmx`
    *   This file shows how to replace the perfect lens with real glass lenses without breaking the design. The key steps involve adding a powerless "dummy" lens (infinite radius). Then, optimizing using the `PMVA` operand to transfer optical power from the paraxial to the real lens. Safely deleting the now-redundant paraxial lens.

### 9. Ritchey-Chrétien Telescope with Corrector
*   **File:** `RC_Lens.zmx`
*   **Description:** A telescope design using two mirrors with special shapes (conic constants). It also uses a group of lenses to correct the final image. The design has very high (diffraction-limited) performance and fits inside a 90mm x 90mm x 170mm box. It is an F/3.31 system.

## Software Requirements

*   These files are made for **Zemax OpticStudio**.
*   You can open them with the free [Zemax OpticStudio Viewer](https://www.zemax.com/pages/opticstudio-viewer) if you do not have a full license.

## Credit

These designs are inspired by the excellent educational videos from Mark Nicholson on the [Design Optics Fast YouTube channel](https://www.youtube.com/@DesignOpticsFast).

## License

This project is for educational purposes.
