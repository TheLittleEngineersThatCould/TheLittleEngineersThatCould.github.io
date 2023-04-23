---
title: "Simulations"
excerpt: "Details of the simulations we ran in NEXTRUCAD to determine screw parameters"
classes: wide

---

To determine the optimal parameters for the screw of our extruder, we used NEXTRUCAD simulation software. NEXTRUCAD simulates single-screw extrusion. We use NEXTRUCAD to determine whether a theoretical extruder will fully melt a polymer and produce filament before building the extruder itself Additionally, the results of NEXTRUCAD allow us to properly size the motor, gearbox, and heaters and determine an economic feasibility analysis before investing any capital into an extruder project

The first step in determining the viscosity data for the polymer that you are looking to extrude. PET is a non-Newtonian fluid meaning its viscosity varies with shear in a Power Law relationship shown here:

$$η=m_{0}*e^{-b(T-T_{R})}\dot{γ}, η<η_{T}*e^{-b(T-T_{R})}  (1)$$

where η is viscosity, m<sub>0</sub> is the consistency at T<sub>R</sub>, T<sub>R</sub> is the reference temperature, b is the temperature sensitivity, γ̇ is the shear rate, n is the Power Law index, and η<sub>T</sub> is the plateau viscosity. By fitting the data developed by Bata et al to equation (1), we were able to determine the values of m<sub>0</sub>, b, and n with a reference temperature of 270 ℃ as shown in Table 1.





