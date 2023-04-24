---
title: "Simulations"
excerpt: "Details of the simulations we ran in NEXTRUCAD to determine screw parameters"
classes: wide

---

To determine the optimal parameters for the screw of our extruder, we used NEXTRUCAD simulation software. NEXTRUCAD simulates single-screw extrusion. We use NEXTRUCAD to determine whether a theoretical extruder will fully melt a polymer and produce filament before building the extruder itself Additionally, the results of NEXTRUCAD allow us to properly size the motor, gearbox, and heaters and determine an economic feasibility analysis before investing any capital into an extruder project

The first step in determining the viscosity data for the polymer that you are looking to extrude. PET is a non-Newtonian fluid meaning its viscosity varies with shear in a Power Law relationship shown here:

$$η=m_{0}*e^{-b(T-T_{R})}\dot{γ}, η<η_{T}*e^{-b(T-T_{R})}  (1)$$

where η is viscosity, m<sub>0</sub> is the consistency at T<sub>R</sub>, T<sub>R</sub> is the reference temperature, b is the temperature sensitivity, γ̇ is the shear rate, n is the Power Law index, and η<sub>T</sub> is the plateau viscosity. By fitting the data developed by Bata et al to equation (1), we were able to determine the values of m<sub>0</sub>, b, and n with a reference temperature of 270 ℃ as shown in Table 1.

**Table 1.** Power Law Parameter Values
<iframe width="228" height="218" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


As noted by other groups, PET extrusion generally works best with high compression screws (3.0:1 to 3.25) with a length around 24 screw diameters.[^1] Based on this knowledge and the difficulty of machining a custom screw, the team decided to purchase the [High Compression Screw](https://www.google.com/url?q=https://www.filabot.com/products/ex6-extruder-screws?variant%3D12866208235554&sa=D&source=docs&ust=1682202980989892&usg=AOvVaw2QnGosJ6nPFrzTRxqXBraR). Using the screw specifications from Filabot, we started to use NEXTRUCAD to design and simulate the remaining portions of the extruder. 

All of the NEXTRUCAD inputs are summarized in Tables 2 - 7. The key results from the simulation can be found in Table 8. The outputs in Table 8 inform everything from our [economic analysis](https://thelittleengineersthatcould.github.io/portfolio/Process_Economics/) to our equipment sizing (LINK HERE).

**Table 2.** NEXTRUCAD Screw (i) Inputs
<iframe width="207" height="189" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=547125923&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


**Table 3.** NEXTRUCAD Screw (ii) Section 1 Inputs
<iframe width="240" height="242" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=231049382&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


**Table 4.** NEXTRUCAD Screw (ii) Section 2 Inputs
<iframe width="240" height="252" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=1163815703&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


**Table 5.** NEXTRUCAD Screw (ii) Section 3 Inputs
<iframe width="240" height="252" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=1052581461&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


**Table 6.** NEXTRUCAD Barrel + Die Inputs
<iframe width="239" height="273" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=695171395&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


**Table 7.** NEXTRUCAD Process Conditions Inputs
<iframe width="267" height="281" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=69842378&amp;single=true&amp;widget=true&amp;headers=false"></iframe>


**Table 8.** NEXTRUCAD Key Results
<iframe width="240" height="294" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQIrFBwUo9KrBYuPAFEcMKQ6K_i5Ti_DNRUJXg2XSECzRbRiSPQHBDpLJvwbxe09tSX9isg1rvm6y7C/pubhtml?gid=1483443242&amp;single=true&amp;widget=true&amp;headers=false"></iframe>



[^1]: M. Bustos Seibert, G. A. Mazzei Capote, M. Gruber, W. Volk, and T. A. Osswald, “Manufacturing of a pet filament from recycled material for material extrusion (MEX),” Recycling, vol. 7, no. 5, p. 69, 2022.
