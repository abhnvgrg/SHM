**README — Mass-Spring SHM Simulation Project (Versions 1 to 6)**

**Overview**
This project simulates Simple Harmonic Motion (SHM) of a mass-spring system using JavaScript and p5.js, evolving through six versions (v1–v6). It progressively enhances the physics modeling, visualization, user controls, and feature set, culminating in a rich interactive simulation with multiple masses, damping, nonlinear springs, external forces, and even a placeholder for quantum simulation.

**Version Progress Summary
Version 1 — Basic Single Mass-Spring Oscillator**
Features:

Simulated a single mass attached to a spring using basic SHM equation 
𝑚
𝑦
¨
+
𝑘
𝑦
=
0
m 
y
¨
​
 +ky=0.

Visualization included a simple mass block oscillating vertically on screen.

Limitations:

No user controls or parameter adjustments.

No damping, forcing, or multiple masses.

Purpose:

Proof of concept and visualization of fundamental SHM.

**Version 2 — User Input for Parameters**
Features:

Added HTML input fields for mass (m) and spring constant (k).

Users could now adjust these parameters dynamically.

Visualization updated accordingly.

Limitations:

Still limited to a single mass.

No damping or forcing yet.

Improvements:

Introduced basic UI, making the simulation interactive.

**Version 3 — Inclusion of Damping and External Forcing**
Features:

Added damping coefficient (b) input.

Added external periodic forcing: force amplitude (F₀) and frequency (ω).

Equation extended to 
𝑚
𝑦
¨
+
𝑏
𝑦
˙
+
𝑘
𝑦
=
𝐹
0
cos
⁡
(
𝜔
𝑡
)
m 
y
¨
​
 +b 
y
˙
​
 +ky=F 
0
​
 cos(ωt).

Improvements:

More realistic physics: energy dissipation and driven oscillations.

Visualization:

Oscillation amplitude responded dynamically to damping and forcing parameters.

**Version 4 — Multiple Masses and Springs (Mass Chain)**
Features:

Allowed simulation of multiple masses connected in series by springs (up to 4 masses).

Implemented system of coupled differential equations.

Used numerical integration (Runge-Kutta 4) for time evolution of the system.

Improvements:

More complex and realistic physics, including interactions between masses.

Extended visualization to display multiple masses and springs dynamically.

Challenges:

Increased computational complexity.

Visual representation of springs with sinusoidal wave shape for better aesthetics.

**Version 5 — Nonlinear Spring and Gravity Effects**
Features:

Added option to enable nonlinear spring behavior via cubic term with coefficient α.

Added gravity effect based on selectable celestial bodies (Earth, Moon, Mars, etc.).

Updated forces and equations accordingly: nonlinear restoring force and gravitational potential included.

Improvements:

Significantly enriched the physical realism of the simulation.

Users can explore non-ideal spring behavior and environmental gravity differences.

Visualization:

Added graphs for position vs. time and energy components (kinetic, spring potential, gravitational potential).

**Version 6 — Final Refinements and Additional Features**
Features:

Polished UI and styling for user-friendly control panel sidebar.

Added simulation mode selector with placeholder for "Quantum" mode (non-functional but prepared).

Energy graphs improved and color-coded for clarity.

Added data export feature (CSV) for position and energy data over time.

Displayed real-time equation and status of each mass (position and velocity).

Enabled restart functionality to update simulation with new parameters instantly.

Technical Improvements:

Refined RK4 integration implementation for system of masses.

Optimized performance with history trimming to keep graph data manageable.

Enhanced spring visualization with sinusoidal waves between masses for aesthetics.

User Experience:

Responsive layout with sidebar and main canvas area.

Intuitive controls for physics parameters, nonlinearities, and gravity environment.

Real-time feedback with equations and status readouts.

Limitations:

Quantum mode not yet implemented.

Export limited to classical mode data.

**General Technical Notes**
Physics Modeling:

The simulation models vertical motion of masses connected by springs under Newtonian mechanics.

Incorporates damping and external forcing.

Nonlinear restoring forces modeled by adding cubic terms to spring force.

Gravity modeled as constant acceleration depending on selected celestial body.

Numerical Integration:

Fourth-order Runge-Kutta (RK4) method used for numerical stability and accuracy.

State vector includes position and velocity of all masses.

Forces computed at each time step for integration.

Visualization:

p5.js handles rendering, including springs as sinusoidal curves and masses as rectangles.

Graphs for displacement and energies provide insight into system dynamics.

UI:

HTML and CSS create a fixed-width sidebar for controls and main canvas for visualization.

Inputs include numeric fields, dropdowns, checkboxes, and buttons.

Real-time updates triggered on parameter changes and restart button.

Data Export:

Simulation data (time, position, kinetic, potential energies) exportable as CSV for further analysis.

**How to Use (v6)**
Adjust parameters in the sidebar:

Choose simulation mode (currently only classical works).

Select number of masses (1-4).

Set mass, spring constant, damping coefficient, external force amplitude and frequency.

Enable nonlinear spring and set nonlinear coefficient if desired.

Select gravity environment from dropdown.

Set quantum number n (placeholder).

Click Restart Simulation to apply new settings.

Observe the simulation animation and energy graphs.

Optionally, click Export CSV to save data from the classical simulation.

**Conclusion**
This project progressively builds from a simple single-mass SHM model into a flexible, interactive multi-mass nonlinear spring system simulator with realistic physics and user-friendly controls. The final version (v6) balances complexity and usability, providing a rich educational tool for visualizing and analyzing mass-spring dynamics under various physical conditions.
