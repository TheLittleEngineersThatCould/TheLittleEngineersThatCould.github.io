---
title: "Wiring"
excerpt: "Summary and diagram of the wiring of our extruder"
classes: wide

---

To complete our extruder, our team wired a variety of parts. The diagram shown below in figure 1 illustrates the flow of our wiring and all necessary components. The extruder receives current from a wall outlet, and splits it into three multiple streams using terminal strips. There is a terminal strip for live, a strip for neutral, and a strip for ground. Some current goes to the VFD, which controls the motor. Some current goes to cooling fans controlled by PWM knobs, which accept 12 V so the current must pass through converters first. The rest of the current goes to PID controllers, where the current temperature is measured by thermocouples and the desired temperature is controlled with heaters. After initially wiring all PID controllers and all fans separately, we decided to daisy chain them because it made cable management easier, reduced the risk of any wire touching the barrel insulation, and allowed for easier removal of the top housing panel.

**Figure 1.** Wiring Logic Diagram
