---
title: "Safety, Health, and Environmental Concerns"
excerpt: "Outlining some important considerations we took into account when building our extruder"
classes: wide

---

## Safety, Health, and Environment Concerns

Both the process of producing regrind flake and operating the filament extruder present environment, health, and safety concerns (EHS). From an environmental perspective, concern may arise around the general nature of filament 3D printing, in that the process generates quite a bit of waste.[^1] The waste produced from filament 3D printing is largely attributed to failed prints or design iterations. This environmental concern could hopefully be mitigated due to the nature of our design. Any failed prints could be processed in the same manner as the recycled plastic bottles: ground up in the granulator into regrind flake, extruded into filament, and pelletized. From here, the failed prints are now considered rPET pellets. However there are limitations to this solution because each time prints are used as a regrind source, they experience mechanical stress from the reclaimer and additional thermal degradation from the extruder. Essentially, the reuse of rPET parts as regrind should not be a regular process, and we aim to rework 10% or less of failed prints back into the regrind stream.

As for health and safety risks, these can be mitigated with the adherence to OSHA regulations set for the plastics industry.[^2] The main health concern arises from the regrind making process. The input to the reclaimer is plastic shreds, while the output is varying sized regrind flake. A substantial portion of the regrind flake is the size of flecks (slightly larger than particles). The flake size can be seen in Figure X below. The flecks also tend to either stick to the internal wall of the regrind due to static attraction or float around in the air. Hazards regarding the regrind and the reclaimer are eye hazards and inhalation hazards.  These hazards can be mitigated by wearing relevant personal protective equipment (PPE) like dust masks and safety glasses. The process of granulating plastics like PLA and ABS have also have hazards with regards to the release of toxins during this process. However, PET is inert so toxin release is not a concern.[^3]

![Reclaimer](/assets/img/Reclaimer.png)
**Figure 1.** Close up view of concerning regrind flake size on reclaimer wall.

Unlike the environmental and health risks, safety concerns are more flagrant in number and consequences. A Hazard and Operability Analysis (HAZOP) and Failure Mode and Effects Analysis (FMEA) were conducted on the filament extruder. To summarize, the greatest safety concerns are rooted in deviations in barrel pressure, loose electrical connections, and exposed rotating machinery. Deviations in barrel pressure can result from a variety of mishaps with regards to operation conditions. If the barrel pressure is too low, this is an indication that there is no melt flow through the barrel, which can result in galling. The safeguard in place is the activation of the emergency stop button, which will kill all of the power to the extruder. If the barrel pressure is too high, the barrel could rupture or explode, which is the greatest safety concern. The safeguard in place is a shear plate that will break and absorb the force if the screw begins moving backward due to pressure build up. The electrical connections, especially the temperature PID controllers and fan PWMs, can pose a safety concern in the case that the loose connections can inaccurate and/or inadequate temperature readings and cooling speeds. Electrical units and components always pose the risk of electrocution and damage to the machinery. Again, the safeguard in place is the activation of the emergency stop button if the PID controllers begin reading values outside the temperature range limits or visual inspection of the extruder indicates an electrical malfunction. Lastly, there is an opening for the hopper where the plastic pellets are fed to the feed section. There is a risk that operators' clothing, hair, or body parts get caught in the screw, which could result in fatality. To mitigate this risk, operator’s should not wear loose clothing and tie their hair back. The hopper should be covered with the lid when pellets are not being fed into the extruder.

## HAZOP

<iframe width="100%" height="1394" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTJaogoAmtnWb0WK2GNmKcRgHxqkhYSXXVIP5gpT0dOP-80XspBVlETEfMoz_Dwgm07rdWo5rUj_CVN/pubhtml?widget=true&amp;headers=false"></iframe>

## FMEA

<iframe width="100%" height="1250" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTYP9uVihe8FQUZ9sfZukBOjD19bdEGUUnp_G4aY2md8NmTbs6al3tD-NRtmII8iw/pubhtml?widget=true&amp;headers=false"></iframe>

## Lock Out Tag Out Instructions

The Lock Out Tag Out form can be downloaded [here][1]. The procedures should be reviewed annually by the EHS manager. 

[1]:{{ site.url }}/Extruder_LOTO.docx

[^1]: Mikula, K., Skrzypczak, D., Izydorczyk, G. et al. 3D printing filament as a second life of waste plastics—a review. Environ Sci Pollut Res 28, 12321–12333 (2021). https://doi.org/10.1007/s11356-020-10657-8

[^2]: “Machine Guarding : Plastics Machinery - Horizontal Injection Molding Machines,” United States Department of Labor. [Online]. Available: https://www.osha.gov/etools/machine-guarding/plastics-machinery/horizontal-injection-molding-machines. [Accessed: 12-Apr-2023]. 

[^3]: “Comprehensive guide on polyethylene terephthalate (PET),” Polyethylene Terephthalate (PET) - Uses, Properties &amp; Structure, 2023. [Online]. Available: https://omnexus.specialchem.com/selection-guide/polyethylene-terephthalate-pet-plastic. [Accessed: 12-Apr-2023]. 



