---
title: "Process Economics"
excerpt: "Assessment of the TCI and payback period of our extruder"
classes: wide

---

## Introduction

A key aspect of any proposed process is the economic viability of said process. The benefits of the design must outweigh the costs. In considering the economic feasibility of our prototype extruder, we must consider three aspects: capital investment, production costs, and sales revenue. With these three aspects, we are able to determine the return on investment for our prototype extruder. However, we must also consider the context of our extruder in comparison to a typical, commercially-available filament extruder such as Filabot’s Standard Series EX6 Filament Extruder. Our extruder is economically viable only if the readily available alternatives are not as financially savvy as our prototype. In addition, the standard profitability analysis does not make logical sense in the context of our project. Our extruder is built for students interested in sustainability and prototyping through additive manufacturing; therefore, for the economic analysis of our extruder, we will consider two different cases. In one case, we will simulate running the extruder as if we are retrofitting the Digital Fabrication Lab with our extruder to produce polymer to sell for a profit. In the other case, we will simulate the savings generated when filament is produced on an as-needed basis. 

**Table 1.** Capital investment of each section of the prototype extruder. The full lists of individual components and their costs can be found in the [Equipment List and Unit Descriptions](LINK) section.
<iframe width="478" height="436" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSrHN7wJ3KYsXJAE4LROnckK29-K7e8XuwEgclLIfXCx6t6EhtOrRsNxZjna8shbD6ND8GjQGMRxEdV/pubhtml?gid=928885553&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

## Capital Investment

Capital investment refers to the cost of the equipment that went into building the prototype extruder. Most analyses of total capital investment are estimates, and analysts go through several different methods of varying degrees of specificity in order to determine the total capital investment. However, for our extruder, we are able to make a definitive estimate because we both designed and built our extruder. Table 1 lists the categories of devices within the extruder along with the actual dollar amount spent on each set of devices. The Motor Train equipment refers to the motor, the gear box, the output shaft, coupler, screw, and die. Electrical equipment refers to the variable frequency drive, the pulse width modulators, the emergency stop button, the power supplies, the wall power connector, and various wiring apparatus. The Heating/Cooling equipment refers to the heating elements, the thermocouples, the temperature PID controllers, and fiberglass insulation. The Machining equipment refers to the taps, lathe attachments, and raw materials used to machine the barrel and flange. 3D Printing Material refers to the acrylonitrile butadiene styrene (ABS) used to print several components. This cost is negligible due to the low cost of filament and the low mass utilized in fabrication. Finally, the Prototyping Risk cost refers to the costs associated with the team purchasing the wrong items or purchasing too many of a device. For example, the team purchased switches for turning the PIDs on and off, but in our final design, we do not include these switches. This is a risk with any prototyping project. Designs change throughout the process leading to extraneous costs for which we must account.. Since this is the first time this machine has ever been built, changes occur leading to a higher cost than theoretically possible, but in the case of our extruder, the Prototyping Risk cost only amounts to about 7% of the total investment. In addition, this cost disappears for all future projects building this exact extruder due to the availability of the CAD model and full equipment list. This cost is just a reminder that this project is a learning experience for the team and that it is important to include room for error when proposing budgets to future employers. 

**Table 2.** The values of key cost and revenue sources. 
<iframe width="633" height="198" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSrHN7wJ3KYsXJAE4LROnckK29-K7e8XuwEgclLIfXCx6t6EhtOrRsNxZjna8shbD6ND8GjQGMRxEdV/pubhtml?gid=1130734118&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

## The “Commercial” Approach

While our extruder has been built for a lab presence, there is value in analyzing the ability to commercialize the extruder for profit. For this simulation, we make the following assumptions:

*  the extruder is being run out of the Digital Fabrication Lab meaning there are no costs related to property or purchasing of the other unit operations occurring in our process;
*  the extruder is run during the standard Vanderbilt school year which we estimate as 30 weeks per year;
*  the extruder is operated by a single undergraduate student who works the 19 hours per week at $10.00 per hour;
*  power consumption will be charged to the Digital Fabrication Lab at a rate of $0.1065 / kWh;
*  the business is being run through Amazon sale thus incurring Amazon’s storage, fulfillment, and referral fees as listed in Table 2; and
100% of our product is usable and sold.

Following these assumptions, we are able to determine the annual revenue of this extruder to be about $33,000 and the annual costs to be about $28,000. Therefore, the profit of the prototype is $5,000 per year. With a total capital investment of $5,433 and a profit of $5,000 per year, the payback period for the prototype extruder is just over a year. However, if the cost of the extruder is instead considered to be a loan of $5,433 at an 11% interest rate, the time required to pay back the loan is 3 years and 7 months. The loan repayment period is determined by equation (1):

$$N = \frac{-ln(1-(P*\frac{APR}{12})/MP)}{ln(1+\frac{APR}{12})}    (1)$$

where N is the number of monthly payments, P is the principal, APR is the annual percentage rate, and MP is the monthly payment. For this simulation, the monthly payment is determined to be 36% of the monthly profit because for small businesses to be considered viable for future loans their debt-to-income ratio, or the percent of monthly income that goes to paying debt, should be 36% or less[^1]. If we compare this result with the case in which we instead purchase Filabot’s Standard-Series EX6 Filament Extruder with a high compression screw, we find that the payback period is just under 3 years due to the EX6 having roughly the same output capacity as our prototype but costs nearly 3 times as much at $15,187. If we run the same loan analysis with the cost of the EX6 with all other variables held constant, we find that it would take 21 years and 5 months to pay off the loans which is over six times as long as the repayment schedule of the prototype extruder.

In both the analysis of the payback period and the loan repayment schedule, we see that the initial cost of the extruder is paid off very quickly when the filament is sold for profit. In order for a business to take part in any process, the process needs to make money. The prototype extruder both makes money and reduces the environmental impact of single-use plastics on Vanderbilt’s campus.

## The “As Needed” Approach

While it is important to consider the potential profitability of our plastic extruder, it is not realistic. Because of the bottleneck of creating regrind and size of filament demand on campus, the extuder will rarely be operated at its maximum capacity. A more realistic analysis of the economic viability of the extruder is to consider the cost savings incurred by printing recycled filament on campus in comparison to buying filament from some outside manufacturer. For this simulation, we make the following assumptions:

*  the Digital Fabrication Lab uses about 30 kg of PETG filament per year and will switch over completely to the Vanderbilt-sourced rPETG filament;
*  the electrical cost to run the extruder is negligible;
*  and the extruder will be run by an unpaid undergraduate student.

In order to purchase 30 kg of PETG filament, it would cost $31.50 per kg amounting to $945 per year in filament alone . However, to produce the same amount of filament using the extruder would only cost $169 per year since the only production cost to consider is the price of pellets, and the cost of the pellets is reduced by 25% due to the presence of the free rPET regrind sourced from Vanderbilt’s plastic waste stream.  Therefore, using the polymer extruder would save the Digital Fabrication Lab $776 per year meaning the savings would overcome the initial investment in the extruder in 7 years. 

[^1]: C. B. Murphy, “Debt-to-income (DTI) ratio: What's good and how to calculate it,” Investopedia, 11-Jan-2023. [Online]. Available: https://www.investopedia.com/terms/d/dti.asp. [Accessed: 17-Apr-2023]. 



