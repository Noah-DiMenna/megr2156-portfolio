# A2 – Truss Stress Analysis

## Note to Reader

Any hand drawn work in this assignment includes standardized highlighting colors:

- **Yellow** highlight signifies the header of a new portion of work (ie: solving for forces, List of Numerical Forces, etc.)

- **Blue** highlight signifies the answer to a question that was being solved under a yellow header (ie: By=-6.66 KN under the yellow header of solving for external forces)

- **Green** highlight signifies commentary, which will also be written as text within this assignment

## Objective

-Design a lightweight planar truss using A500 steel or an alternative material.

-Create free body diagrams (FBDs) for joints and critical pins.

-Calculate the required cross-sectional area of truss elements with a safety factor.

-Determine pin sizes based on shear forces with a safety factor.

-Solve equations symbolically and numerically for both truss and pin design.

-Estimate the total weight of the truss and pins.

-Create a CAD model with accurate dimensions and connections.

-Compare CAD weight predictions with hand calculations.

-Document key engineering lessons learned from the process.

## Analyze

# My Process

For Assignment A2 I was tasked with creating a planar truss that fit within given parameters. 

<img src="Given-Layout.jpg" style="border-radius: 12px; width: 75%;">

This was the layout given to design a truss to support:

- **Point A** is a pin support

- **Point B** is a horizontal roller support

- **Point C**  is where the first P force is located

- **Point D** is where the second P force is located

## 2. Designing Truss Structure

**a. Design the truss structure using parameters in Figure #1**

**i. Sketch a truss structure by generating the lengths of each element based to support the loads at point C and D.**

<img src="A2-Base-Layout.jpg" style="border-radius: 12px; width: 50%;">

I started by making a basic layout to standardize each of my following designs. This would make it easier to compare the designs and make an informed decision on which one would work best for the presented problem. 

## Preliminary Designs

I came up with 3 different designs that could work as a viable solution to supporting both forces and points C and D

Design 1:

<img src="A2-Design1.jpg" style="border-radius: 12px; width: 50%;">

This is a simple underbody truss that directly connects point B to point C, connects point A to point D, connects C and D, and makes a new point "E" that all points meet at in the middle. 

Design 2:

<img src="A2-Design2.jpg" style="border-radius: 12px; width: 50%;">

This design Prioritized supporting both loads at points C and D from both anchor points A and B. A support connects both C and D to point B, as well as two supports connecting both loads to point A. One additional member connects the Loads together to make the structure stable.

Design 3:

<img src="A2-Design3.jpg" style="border-radius: 12px; width: 50%;">

This design utilized the fact that both P forces are perfectly vertical, so both forces would be transmitted directly through their member to a strong truss assembly above points A and B. 

## Picking a Design

Overall Design 1 made the most sense to use because it was the most simple of the 3, and would most likely have the best dispersion of both forces through all of the members, so it was the one I continued the engineering process with going forward. Both design 2 and 3 would pose problems with individual members of the truss taking on too much of the overall load P from both point C and D. Design 1 also will give the best strength to weight ratio since it will be far lighter than design 3 and have overall shorter members than design 2. 

## ii. Design 1 Freebody Diagram

<img src="A2-Design1-FBD.jpg" style="border-radius: 12px; width: 50%;">

This is the freebody diagram of the design I chose to move on with. It include a separate diagram for each join A through E, including external forces where necessary. These forces include support forces on joints A and B, and load forces P on joints C and D. 

## iii. Symbolically solve for all internal forces

### External Forces:

<img src="A2-External-Sym.jpg" style="border-radius: 12px; width: 75%;">

These are solving for the external (support) forces of my truss, solved symbolically. 

**B<sub>y</sub>= - $\frac{1}{3}$ P**

**A<sub>y</sub>= $\frac{1}{3}$ P**

### Internal Forces:

<img src="A2-JointB-Sym.jpg" style="border-radius: 12px; width: 30%;">

From joint B we find:

**F<sub>BC</sub>= - $\frac{5}{9}$ P**

**F<sub>BE</sub>= $\frac{4}{9}$ P**

<img src="A2-JointC-Sym.jpg" style="border-radius: 12px; width: 50%;">

From joint C we find:

**F<sub>CE</sub>= - 0.8012 P**

**F<sub>CD</sub>= 0 P**

Reminders:

There are multiple cosines used in finding **F<sub>CD</sub>**. These are not the same cosine value as they both come from different angles within the truss. The cosine being multiplied by **F<sub>CE</sub>** is equal to **$\frac{0.2}{\sqrt{0.13}}$**. And the cosine multiplied by **F<sub>BC</sub>** is equal to **0.8**.

Member **F<sub>CD</sub>** does not have any internal force, so it could be removed in theory. But considering the fact that this only happens because the system is in perfect equilibrium, it would completely fail if any change were to happen to the system and member **F<sub>CD</sub>** not being in the system. Because of this I chose to keep the member moving forward.  

<img src="A2-JointA-Sym.jpg" style="border-radius: 12px; width: 30%;">

From joint A we find:

**F<sub>AD</sub>= $\frac{5}{9}$ P**

**F<sub>AE</sub>= - $\frac{4}{9}$ P**

<img src="A2-JointD-Sym.jpg" style="border-radius: 12px; width: 30%;">

From joint D we find:

**F<sub>DE</sub>= 0.8012 P**

### List of Symbolic Forces:

<img src="A2-List-Sym.jpg" style="border-radius: 12px; width: 20%;">

This is a combined list of all forces found symbolically in the last step. 

### Numerically Solving for Forces

<img src="A2-Num-Solving.jpg" style="border-radius: 12px; width: 50%;">

Since all of these forces were solved symbolically beforehand, solving for them numerically is as easy as plugging in what value was decided for the force **P** at the beginning. I chose **20KN** for my force **P**. 

From this step we find the following: 

**B<sub>y</sub>= - 6.666KN**

**A<sub>y</sub>= 6.666KN**

**A<sub>x</sub>= 0KN**

**F<sub>AE</sub>= - 8.888KN**

**F<sub>AD</sub>= 11.111KN**

**F<sub>BE</sub>= 8.888KN**

**F<sub>BC</sub>= - 11.111KN**

**F<sub>CE</sub>= - 16.025KN**

**F<sub>CD</sub>= 0KN**

**F<sub>DE</sub>= 16.025KN**

### List of Numerical Forces:

<img src="A2-List-Num.jpg" style="border-radius: 12px; width: 20%;">

This is a combined list of all numerically solved forces given that **P = 20KN**, found in the last step. 

## Finding Cross-Sectional Area of Members

<img src="A2-MemberCSA-Var.jpg" style="border-radius: 12px; width: 60%;">

The above image shows a list of known and unknown variables that pertain to finding the minimum cross-sectional area. These variables include:

#### Known Variables:

Largest internal forces:

**F<sub>CE</sub>= - 16.025KN**

**F<sub>DE</sub>= 16.025KN**

Safety Factor = 3.5

Yield strength of A500 structural steel: (**Y<sub>ss</sub>= 269MPa**

#### Unknown Variables:

Minimum Cross-Sectional area (**AY<sub>min</sub>**)

Max Stress

Yield strength (before finding it on google)

<img src="A2-Amin-Sym.jpg" style="border-radius: 12px; width: 50%;">

This is the math that symbolically solves for **A<sub>min</sub>**

From this we find:

**$A_{min} = P \frac{SF}{S_y}$**

<img src="A2-Amin-Num.jpg" style="border-radius: 12px; width: 50%;">

Here takes the equation found in the last step and uses it to solve for $A_{min}$ by plugging in the known values to the right side of the equation. 

This gives us:

**$A_{min} = 208.5037mm^2$**

 or

 $A_{min} = 0.0002085m^2$

<img src="A2-Member-Vol.jpg" style="border-radius: 12px; width: 50%;">

This step takes the cross-sectional area found in the last step and multiplies it by the length of each member to find its volume. This is done in preparation to find the mass of each member in the next step. The density of A500 structural steel is also noted here in preparation for the next step. 

From this step we find that:

$V_{BE}=V_{AE}=1.25x10^{-4} (m^3)$

$V_{CD}=8.34x10^{-5} (m^3)$

$V_{BC}=V_{AD}=1.0425x10^{-4} (m^3)$

$V_{CE}=V_{DE}=1.25x10^{-4} (m^3)$

<img src="A2-Member-Mass.jpg" style="border-radius: 12px; width: 50%;">

Using the Information from the previous photo, everything needed to find the mass of each member is now available. 

From this we find that:

$m_{BE}=m_{AE}=0.982035 (Kg)$

$m_{CD}=0.65469 (Kg)$

$m_{BC}=m_{AD}=0.8183625 (Kg)$

$m_{CE}=m_{DE}=0.59012 (Kg)$

<img src="A2-Member-Mass-List.jpg" style="border-radius: 12px; width: 50%;">

This photo expands the mass of each member to more clearly state the weight of each truss member. 

<img src="A2-Member-Total-Mass.jpg" style="border-radius: 12px; width: 50%;">

This calculates the total mass of the truss system by adding up the mass of each member into one combined value.

This gives us:

$m_{total}=5.4357 (Kg)$

## Finding Cross-Sectional Area of Connecting Pins

<img src="A2-Pin-CSA-Var.jpg" style="border-radius: 12px; width: 50%;">

This picture covers known quantities needed to find the cross sectional area of the pins that connect each member of the truss to each other.

<img src="A2-Pin-Unit-Conversion.jpg" style="border-radius: 12px; width: 50%;">

This converts the given units to metric so that they can be used with previously obtained units. 

<img src="A2-Pin-FBD.jpg" style="border-radius: 12px; width: 50%;">

This is the freebody diagram for both pins with the largest loads on them, Pin C and Pin D.

<img src="A2-Pin-Amin-Sym.jpg" style="border-radius: 12px; width: 25%;">

This image shows the conversion done in order to symbolically solve for $A_{min}$

<img src="A2-Pin-Amin-Num.jpg" style="border-radius: 12px; width: 25%;">

This uses the equation found in the previous image to find $A_{min}$ by plugging in all of the known values into the equation.

Doing so gives us:

$A_{min}=0.00006825 (m^2)$

<img src="A2-Pin-Length.jpg" style="border-radius: 12px; width: 50%;">

This equation gives the length that each pin has to be. The answer is also the length of all sides of each truss which will be used in the CAD modeling further on. 

This gives us:

$L_{Pin}=0.0144 (m)$

<img src="A2-Pin-Mass.jpg" style="border-radius: 12px; width: 50%;">

This image shows the steps to find the mass of each pin for the truss system. First the volume of the pin is found, then using the volume and density, Pin mass is found. 

The step gives us:

$m_{Pin}=0.00757 (Kg)$

<img src="A2-Pin-Mass-Total.jpg" style="border-radius: 12px; width: 50%;">

This image shows multiplying the pin mass by 5 to compute the total mass of all 5 pins combined. 

Which gives us:

$m_{PinTotal}=0.0378 (Kg)$

<img src="A2-Pin-Diameter.jpg" style="border-radius: 12px; width: 50%;">

Finally the diameter of the pins must be found before moving into Cad to generate our design. 

performing the equations above gives us:

$d=0.00932 (m)$

This step was not necessary before to find the volume and mass of the pins because we already knew the cross sectional area, it is however needed to create a CAD version of the pins in the next step. 

## CAD Model

### Base Layout:

<img src="A2-CAD-Layout.png" style="border-radius: 12px; width: 50%;">

This is the preliminary sketch I made as the layout of for my truss. All measurements are in meters, and the 3D modeling software I chose to use was OnShape. I created a point where Pin E was to be located, with a vertically constrained construction line in the middle that measures down $0.3m$. Directly to the left is a point that is measured to be $0.6m$ away, this will become Pin B. Another point is place $0.2m$ to the left of the bottom of the construction line, this pin will become Pin C. Finally Points B and C are mirrored about the construction line to create points A and D respectively. 

### Part 1: Members Only 

<img src="A2-CAD-Member-Photo.png" style="border-radius: 12px; width: 75%;">

This is a photo of my 5 members after creation. All members have the same cross-sectional area of $A_{min}=0.0002085m^2$, and their own respective lengths as shown in the diagram above. 

<img src="A2-CAD-Pin-Picture.png" style="border-radius: 12px; width: 75%;">

This photo shows the 5 pins at their respective spot, each has the same depth (length) as the truss members, and a diameter of $d=0.00932m$. 

### Truss mass

<img src="A2-CAD-Member-Weight.png" style="border-radius: 12px; width: 50%;">

This photo shows the combined weight of the members within the CAD file. Keep in mind that the proper material (A500 Structural Steel) has to be applied to each member before this measurement can be taken, If this step is not done, weight measurements will not be correct. 

From this we find:

$m_{CADmembers}=5.429Kg$

<img src="A2-CAD-Pin-Weight.png" style="border-radius: 12px; width: 50%;">

This photo shows the combined weight of the pins within the CAD file. Just like the members in the last step, the proper material (Hardened Tool Steel) must be applied to all pins before taking this weight measurement. 

From this we find:

$m_{CADpins}=0.038Kg$

### Truss Mass % Difference:

<img src="A2-CAD-Percent-Diff.jpg" style="border-radius: 12px; width: 75%;">

From the calculations above, we see that:

$diff_{members}=0.123$

$diff_{pins}=0.342$

Overall this is a very small difference between 


















## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

