# Lab 3 – Infill and Wall Thickness

## Design

For this lab, I designed a small ring using SolidWorks. I created the ring by sketching two concentric circles with an outer diameter of **1.00 inch** and an inner diameter of **0.80 inch**. I then used Boss-Extrude to give the ring a final height of **0.20 inch**.

I chose this design because it is simple, meets the size requirements of the lab, contains infill, and has no overhangs that would require support material.

The final model dimensions were **1.00 in × 1.00 in × 0.20 in**, which are within the required maximum size of 1.5 in × 1.5 in and maximum height of 0.5 in.

<img width="461" height="378" alt="Screenshot 2026-09-08 at 12 10 23 PM" src="https://github.com/user-attachments/assets/f18a4abb-ff67-4a0c-a82a-ad93373421fc" />


<img width="254" height="341" alt="Screenshot 2026-09-08 at 12 11 36 PM" src="https://github.com/user-attachments/assets/293c47f8-ebbd-49c1-bff7-c2613ac7dd17" />



---

## Research

Three infill patterns I researched were **Gyroid, Cubic, and Adaptive Cubic**.

**Gyroid infill** uses continuous curved shapes throughout the inside of the part. It can provide strength in multiple directions while keeping material use relatively low.

**Cubic infill** creates a three-dimensional repeating structure inside the object. Because the pattern extends in several directions, it can provide good support for functional parts.

**Adaptive Cubic infill** changes the internal structure depending on where support is needed. More material is used near the outside surfaces, while less material is used in larger open areas. This can help reduce printing time and material usage.

### Effect of Infill Percentage and Pattern

Increasing infill percentage generally makes a printed component stronger and stiffer because more material is placed inside the object. However, higher infill also increases filament usage, weight, and print time.

Different infill patterns affect mechanical properties because they arrange material differently and distribute forces in different ways. Two parts with the same infill percentage can still have different strength characteristics depending on the pattern used.

For my design, I used **15% infill with a Grid pattern**. This allowed the ring to have an internal structure while keeping material use and print time relatively low.

---

## Preprocessor and Printing

After completing the model in SolidWorks, I exported it as an STL file and imported it into PrusaSlicer.

The model was prepared using the **Prusa CORE One with a 0.4 mm nozzle**. It remained at **100% scale** and had final dimensions of **1.00 in × 1.00 in × 0.20 in**.

I placed the ring flat on the build plate because this gave it a stable printing surface and eliminated the need for supports. No brim was used because the ring already had enough contact area with the build plate.

The main PrusaSlicer settings used were:

- Infill: **15%**
- Infill Pattern: **Grid**
- Wall Setting: **2 perimeters**
- Approximate wall thickness for 2 perimeter lines: **0.86 mm**
- Layer Height: **0.20 mm**
- Top Solid Layers: **5**
- Bottom Solid Layers: **3**
- Minimum Top Shell Thickness: **0.70 mm**
- Minimum Bottom Shell Thickness: **0.50 mm**
- Scale: **100%**
- Supports: **Not required**
- Brim: **None**
- Material: **PLA**

<img width="280" height="197" alt="Screenshot 2026-09-08 at 12 13 37 PM" src="https://github.com/user-attachments/assets/e0e5afb8-53c7-4e65-bdd3-9adc8434876f" />


<img width="487" height="146" alt="Screenshot 2026-09-08 at 12 12 42 PM" src="https://github.com/user-attachments/assets/a14dce1d-c2c0-4fe1-9dfb-1e086e99a047" />

<img width="414" height="291" alt="Screenshot 2026-09-08 at 11 29 32 AM" src="https://github.com/user-attachments/assets/d7413c00-b9f8-4cb4-b146-8f2735423ba4" />



The sliced preview was checked before printing to make sure the ring contained infill and that the selected settings were applied correctly.

### Wall Thickness

Different wall thicknesses are used because the walls contribute greatly to the strength and durability of a printed part. Thicker walls generally make a component stronger, but they also use more material and may increase printing time.

Thinner walls use less material but may make a part easier to deform or damage. Wall thickness also affects how much room remains inside the object for infill.

For my model, I used **2 perimeters**, which corresponds to an approximate recommended wall thickness of **0.86 mm** at the selected 0.20 mm layer height.

---

## Print

The ring was printed using an FDM printer at the UNCC print farm. The final model met the lab requirements because it was smaller than **1.5 in × 1.5 in**, was only **0.20 in tall**, contained infill, had no overhangs, and did not require supports.

The design also used modified slicer settings, including **15% Grid infill** and **2 perimeters** for the wall setting.

The estimated print time in PrusaSlicer was **20 Minutes**, and the actual print took approximately **25 Minutes**.

<img width="237" height="206" alt="Screenshot 2026-09-08 at 12 14 16 PM" src="https://github.com/user-attachments/assets/502a422e-ab8d-404f-8098-faa629761e47" />

<img width="190" height="157" alt="Screenshot 2026-09-08 at 12 14 37 PM" src="https://github.com/user-attachments/assets/b370a924-91f5-4480-89b2-25b2fd601e58" />


A quick video of my groups Lab 3 print.



https://github.com/user-attachments/assets/b91b6037-ff40-4ca4-8490-8acdc31c01b9



---

## Lessons Learned

This lab helped me understand that the internal structure of a 3D-printed object is important even though it cannot always be seen from the outside. Changing the infill percentage changes how much material is inside the part, while changing the infill pattern changes how that material is arranged.

I also learned that wall thickness can have a major effect on the strength of a component. Thicker walls can make a part stronger, but they also use more material and leave less space for infill.

Using PrusaSlicer showed me the importance of checking the sliced layers before printing. I was able to confirm that the ring actually contained infill and that the settings I selected were being applied correctly.

### Mistakes and Improvements

One mistake I caught was making sure that the ring actually contained infill after adjusting the slicer settings. Because the ring has a relatively small cross-section, the wall settings affect how much space remains for infill.

I checked the PrusaSlicer preview and confirmed that infill was present before sending the model to the printer.

A mistake that could have gone unnoticed would be accidentally using the wrong infill pattern, percentage, wall setting, or material profile. The outside of the model could still look correct even if one of these internal settings was wrong.

In future projects, I would check the dimensions, scale, orientation, material, infill percentage, infill pattern, wall settings, layer preview, and print time before starting the print.

### Scaling the Decision Up

For this small ring, choosing the wrong infill percentage or wall thickness may only result in a weak or failed print. If the same mistake were made on a larger structural or safety-critical component, the consequences could be much more serious.

An infill percentage that is too low or a wall that is too thin could cause a component to deform, crack, or fail when a load is applied. This could cause equipment damage or possibly injury.

This shows why engineers need to consider material, wall thickness, internal structure, and expected forces when designing functional parts.

### Real-World Product Connection

A real-world product that relates closely to my design is a **copper plumbing crimp ring used with PEX tubing**.

I got the idea for the ring from doing plumbing work with my father. When making plumbing connections, we would slide a copper crimp ring around the end of the tubing and fitting. We would then use a hand crimping tool to clamp the ring tightly around the connection.

The thickness and material strength of the ring are important because it must apply enough pressure to keep the plumbing connection secure. If the ring is too thin or too weak, it could deform or fail to hold the connection properly, which could cause a leak.

This connects to the lab because wall thickness, material, and internal structure all affect how well a component handles force. For my printed ring, an incorrect setting may only make the print weaker. For a plumbing connection, an incorrect design or material choice could cause the connection to fail.

---

## Resources

- SolidWorks
- PrusaSlicer
- UNCC FDM Print Farm
- Lab 3 instructions and rubric
- Course lecture and live demonstration
- Prusa Knowledge Base
- ChatGPT – used for assistance understanding infill concepts and organizing the documentation
