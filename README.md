# Mass-Spring Simple Harmonic Motion (SHM) Simulation

## Overview

This project simulates a mass-spring system exhibiting simple harmonic motion (SHM). It numerically solves the system’s differential equations using the Runge-Kutta 4th order (RK4) method for accurate time evolution. The simulation is visualized using p5.js and features interactive UI controls for various physical parameters.

The project evolved through six versions, each adding features, improving numerical methods, and enhancing visualization and user experience.

---

## Version History

### v1: Basic SHM Simulation
- Single mass-spring system without damping or external forces.
- Euler method numerical integration.
- Basic graphical visualization.
- Minimal UI controls.

### v2: Improved Numerical Solver & UI
- Switched to RK4 method for better accuracy.
- UI controls for mass (m), spring constant (k), and initial displacement.
- Real-time position and velocity display.
- Improved layout and styling.

### v3: Multiple Masses & Springs
- Support for up to 4 masses connected in series by springs.
- Interaction forces between connected masses.
- UI allows selecting number of masses.
- Distinct visualization of each mass and spring.
- Added kinetic and potential energy calculations.

### v4: Damping and External Forcing
- Added damping coefficient (b).
- External periodic forcing function \( F_0 \cos(\omega t) \).
- UI inputs for damping and forcing parameters.
- Real-time energy component display.
- Graphs for position and energy over time.

### v5: Nonlinear Spring and Gravity
- Nonlinear spring with cubic term \( \alpha (x)^3 \).
- Gravity effects with selectable celestial bodies.
- UI for nonlinear coefficient and gravity selection.
- Updated force calculations.
- Energy calculations updated.
- Export simulation data as CSV.

### v6: Refinements & UI Polishing
- Finalized UI layout with sidebar controls.
- Sine-wave shaped spring visualization.
- Placeholder for quantum simulation mode.
- Enhanced graphs with legends and grid lines.
- Input constraints and unit consistency.
- Export CSV button added.
- Real-time system equations display.
- Modular code structure.

---

## General Technical Notes

- Numerical integration is performed using the Runge-Kutta 4th order (RK4) method for stability and accuracy.
- Visualization leverages p5.js, allowing dynamic rendering of masses, springs, and graphs.
- UI controls enable real-time parameter adjustments, facilitating exploration of SHM behavior under varying conditions.
- Energy components (kinetic, potential) are calculated and displayed to provide insight into system dynamics.
- The code is modular to allow easy extension for future versions or additional physical effects.
- Export functionality outputs simulation data in CSV format for further analysis.

---

## Conclusion

This progressive simulation project provides an interactive, educational tool for understanding simple harmonic motion and related physics concepts. Through iterative enhancements from v1 to v6, it covers fundamental oscillations, damping, forcing, nonlinearities, and gravity effects, demonstrating both numerical methods and visualization techniques. The project can serve as a foundation for more advanced physical simulations or teaching aids.

