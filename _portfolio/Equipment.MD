---
title: "Materials and Equipment"
excerpt: "Explanation of materials used, sizing of key equipment, and full equipment lists"
classes: wide

---

## Materials

##### Chosen Materials for Construction

For components of our extruder that were made custom by the team, we chose materials that balanced minimizing cost with ensuring satisfactory performance. 

We machined our barrel out of 1144 carbon steel. We chose this steel because it is relatively soft, with a hardness of 22 on the Rockwell C scale. Since we machined the part ourselves, we wanted a softer steel so it would be easier to machine. At one point, we had a concern about the barrel being softer than our screw, which is made of 17-4 PH Stainless Steel Con. H900. This type of steel has a hardness of 40 on the Rockwell C scale.[^1] Our concern was that if the screw were to hit any part of the barrel, it would leave scratches on the inside of the barrel, or potentially even rupture it. To mitigate this concern, we added a bearing to the end of the screw to ensure complete stability on both ends, preventing any collisions between the screw and barrel.

We also machined a flange to connect the barrel to the feed section of our extruder, which is where our hopper is used to funnel in PET flakes. We made the flange and spacer plate out of 12L14 carbon steel, which is a free machining steel alloy, meaning it is easy to machine.[^2]

We ordered custom sheet metal from [SendCutSend](https://sendcutsend.com/?gclid=CjwKCAjw0ZiiBhBKEiwA4PT9zzvO_CfLu9lTMdnaAkZugVP32R8HdzDwb4WKqtKZh6JlM6L2qVQ5RRoCiKYQAvD_BwE) for the housing surrounding our extruder setup, which is present to ensure safety. We chose to make the housing out of aluminum, because aluminum is lightweight, cost-effective, and sufficiently strong for our purposes. The other material option we considered was stainless steel. Although stainless steel is stronger and more rigid than aluminum, we chose aluminum because it is cheaper than stainless steel, and our housing design does not require the added strength of stainless steel. Our housing only needs to support the weight of a few PID controllers and a VFD on top, so we decided aluminum was a perfectly acceptable strength. In order to bolster the strength of our aluminum housing, we also created a frame out of t-slot aluminum extrusions, allowing us not only to add reinforcement to each face of the housing, but also to easily assemble the housing by simply fastening each sheet metal face to the frame.

The other custom parts in our extruder included shrouds for the fans, to direct streams of air to the exact parts of the barrel where they are needed, a hopper to funnel PET flakes into our feed section, and a mount for the power outlet on the side of our housing. We 3D printed these parts in the Digital Fabrication Lab out of ABS. We chose to print these components out of ABS over PLA mainly due to the heat resistant properties of ABS. Since our extruder heats up the barrel to high temperatures, we wanted anything remotely near the barrel to be made out of heat resistant polymers. 

##### Material Used by Device

The most important material pertaining to this project is PET, which is the polymer used to create most plastic bottles, and is therefore the polymer we aimed to recycle using our extruder. When creating filament out of PET, our goal was to create a product that had sufficient material properties to be used for a wide variety of 3D printing applications. 

Mechanical properties of a polymer can be critical to the results of 3D printing when the resulting print needs to be strong or durable. Unfortunately, thermal degradation is a factor that needs to be taken into account when using recycled polymers, such as PET. Thermal degradation is the altering of mechanical properties due to small molecular changes to the polymer that occur at high temperatures. In the case of PET, thermal degradation causes lower viscosity, lower melting point, and lower strength. The mechanism of thermal degradation in PET involves transesterification, the breaking of ester bonds and the formation of new bonds.[^3] 

Our team took the thermal degradation of recycled PET into account in our NEXTRUCAD simulations. Instead of using widely available viscosity data for virgin PET, we searched literature to find viscosity data for recycled PET. Table 1 below shows the viscosity data used in our NEXTRUCAD simulations.

**Table 1.** Viscosity data for recycled PET from literature.[^4] 
<iframe width="300" height="250" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQFYcTZd9KjOMpW4srbrbgWDCMKQVAenGTj7RHRnccXgXv6quyG1Edwb0_3H2teKCVe-glmulCIeioD/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

Another way we investigated the material properties of our recycled PET was by creating a DSC curve. A DSC curve can be used to determine melting point, crystallization temperature, and glass transition temperature. For our purposes, we were only concerned with finding the melting point, since we need all of the PET in our extruder to be melted to avoid clogging the barrel. Figure 1 below shows the DSC curve we obtained from a sample of one of the plastic bottles we used to make regrind. The dip at 250 °C signifies the melting point of the sample which matches the melting point found in literature.[^5]

![DSC curve](/assets/img/DSC.png)
**Figure 1.** DSC Curve from PET regrind

## Equipment Sizing

The specifications of some parts were critical to the extruder running properly. The motor needed to have sufficient horsepower, the heaters and thermocouples needed to be able to achieve and measure a sufficiently high temperature, and the barrel needed to be thick enough to safely withstand the internal pressure.

From [NEXTRUCAD](https://thelittleengineersthatcould.github.io/portfolio/Simulation/), we determined the required torque of our motor to be 0.26 hp. We chose a slightly oversized motor, with ⅓ hp.

From our DSC curve, we determined the melting point of our recycled PET to be 250 °C. Therefore, we chose heaters that are able to easily achieve that temperature, and thermocouples that can easily measure up to and above that temperature. 

Barlow's Law is shown below in equation 1:

$$P = \frac{2𝝈_{Θ}s}{D}$$

The max pressure value was used to determine the required thickness, using Barlow’s Law, where P is the internal pressure, 𝝈Θ is the allowable stress of the material, s is the wall thickness, and D is the outer diameter of the barrel. We chose a barrel thickness of 0.479 in and then used Barlow’s Law to ensure that this selection would produce an allowable stress well below the yield strength of our barrel material. With the barrel thickness of 0.479, a maximum pressure converted to 865 psi, and an outer diameter of 1.109 in, the allowable stress is 1001 psi. The barrel is made from 12L14 steel, which has a yield strength of 60,000 psi. These results signify that our safety factor is around 60, which is exceptionally high.

## Mechanical Assembly

Table 2 below shows a bill of materials for all mechanical parts that we ordered from commercial vendors. The overall cost was $3,075.92.

**Table 2.** Bill of Mechanical Materials.
<iframe width="100%" height="1000" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSrHN7wJ3KYsXJAE4LROnckK29-K7e8XuwEgclLIfXCx6t6EhtOrRsNxZjna8shbD6ND8GjQGMRxEdV/pubhtml?gid=1951519260&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

We used Fusion 360 to create a 3D rendering of our extruder before starting with physical assembly. Please see our [CAD page] for an interactive model of our full extruder assembly and links to pictures and individual CAD models of each mechanical and electrical part we used in assembly. 

## Electrical Assembly

Table 3 below shows a bill of materials for all electrical components of our extruder. The overall cost was $861.22.

**Table 3.** Bill of Electrical Materials.
<iframe width="100%" height= "300" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSrHN7wJ3KYsXJAE4LROnckK29-K7e8XuwEgclLIfXCx6t6EhtOrRsNxZjna8shbD6ND8GjQGMRxEdV/pubhtml?gid=71501716&amp;single=true&amp;widget=true&amp;headers=false"></iframe>



[^1]: “17-4 ph stainless steel bar,” Best Stainless, 2023. [Online]. Available: https://www.beststainless.com/17-4-ph-stainless-steel.html. [Accessed: 24-Apr-2023].

[^2]: “12L14 vs 1018 steel - precision machine technologies,” Spex Precision Machine Technologies, 03-Nov-2022. [Online]. Available: https://www.spex1.com/12l14-vs-1018-steel/. [Accessed: 24-Apr-2023].

[^3]: T. Ma, R. Wang, W. Wang, W. Gu, Y. Yuan, A. Zhang, and J. Wei, “Studies on the thermal degradation mechanism of polyethylene terephthalate and its 2-carboxy ethyl (phenyl) phosphinic acid copolymers,” Polymer Degradation and Stability, vol. 206, p. 110185, 2022.

[^4]: A. Bata, G. Toth, D. Nagy, and K. Belina, “Melt shear viscosity of original and recycled PET in wide range shear rate,” Journal of Physics: Conference Series, vol. 1045, p. 012007, 2018.

[^5]: V. Guarino and L. Ambrosio, Electrofluidodynamic Technologies (efdts) for biomaterials and medical devices: Principles and advances. Duxford, UK: Woodhead Publishing, and imprint of Elsevier, 2018.
