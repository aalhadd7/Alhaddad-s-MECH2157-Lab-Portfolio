# Lab 6 – Parametric Snap-Fit Design

## Artifact Measurements and Initial Planning

For this lab, I designed a small 3D-printed component that would snap fit onto the artifact provided in class. I began by measuring the artifact with calipers so that I could recreate the important mating features in SolidWorks. I recorded the measurements in millimeters and created a hand sketch showing the top, front, and side views of the artifact.

The main measured length of the artifact was approximately 25.53 mm. Other measurements were taken for the width, height, and smaller features that would interact with my printed design. These measurements were used as the starting dimensions for the CAD model.

<img width="470" height="289" alt="Unknown-10" src="https://github.com/user-attachments/assets/c42ba637-311c-404a-8218-1ea45ca235a6" />


---

## Parameters and Design Decisions

The main parameters used in my design were the overall length, width, height, opening dimensions, snap dimensions, wall thickness, and clearance between the artifact and the printed component. I chose these parameters because they directly control whether the component fits onto the artifact and whether the snap features can hold it in place.

I added approximately 0.30 mm of clearance to the mating dimensions. I chose this clearance because a 3D-printed part should not be modeled exactly the same size as the object it fits around. The extra space accounts for small printing variations and gives the part enough room to slide onto the artifact.

The parameters also allowed the design to be changed without completely rebuilding the model. If the fit needed to be tighter or looser, I could adjust the dimensions controlling the clearance and snap features.

---

## Initial SolidWorks Sketch

I began the SolidWorks model by creating the main side profile of the component. The overall length of this profile was 25.83 mm. The outside height was 7.90 mm, and the lower section of the profile was approximately 4.80 mm high. The raised sections at both ends were dimensioned at 3.00 mm.

I used dimensions and geometric constraints to control the sketch. The matching features on each side were kept symmetrical so that the artifact would sit evenly inside the final component.
<img width="982" height="487" alt="Unknown" src="https://github.com/user-attachments/assets/b247d65c-1e53-4b5a-9b03-7f9a0fc5b5ea" />


---

## Creating the Main Body

After completing the main profile, I used Boss-Extrude to turn the sketch into a three-dimensional part. The original extrusion depth was approximately 10.90 mm. This created the basic body of the component before the internal openings and snap-fit features were added.

<img width="2048" height="1105" alt="Unknown-2" src="https://github.com/user-attachments/assets/a6f53916-6e58-48a1-9665-43ac3409be82" />


---

## Creating the Mating Area

I used Cut-Extrude features to remove material from the main body and create the area where the artifact would sit. The shape of these cuts was based on the measurements that I took from the original artifact.

The purpose of this area was to guide the artifact into the component while still leaving enough clearance for the two parts to fit together. The 0.30 mm allowance was considered when creating the mating geometry.
<img width="588" height="633" alt="Unknown-3" src="https://github.com/user-attachments/assets/477d796c-c1f6-42f8-b84d-0f7387197b7b" />


---

## Snap-Fit Design

The next step was creating the snap-fit features. I designed small raised tabs on the sides of the component that would interact with the artifact when it was pushed into place. The angled geometry helps guide the artifact past the snap while the lower portion of the feature helps keep the artifact from being easily pulled back out.

I first created the snap geometry on one side of the component. After the first snap feature was completed, I used the Mirror tool to create the same geometry on the opposite side. Using the Mirror feature kept the snap locations symmetrical and made the model easier to modify.

<img width="851" height="462" alt="Unknown-5" src="https://github.com/user-attachments/assets/4054a808-6b59-4624-bd32-5f51ffd5f9b7" />



---

## Final CAD Design

After creating the snap features, I reviewed the overall model and made a final design change. I increased the thickness of the outside portions of the component to provide better support and improve the strength of the part when it was sliced and printed.

The original outside sections appeared thinner than I wanted for a functional snap-fit component. Increasing the outside thickness gave the model a stronger structure around the mating area while allowing the inside dimensions and snap features to remain based on the measurements of the artifact.
<img width="2048" height="886" alt="Unknown-4" src="https://github.com/user-attachments/assets/73f730b8-0fb2-4326-8fc6-bd550a1f8fa7" />


<img width="851" height="462" alt="Unknown-5" src="https://github.com/user-attachments/assets/71f89117-aaa9-4d26-b73d-20a55882058f" />


The completed SolidWorks model contained the main body, internal mating area, angled transitions, and mirrored snap-fit features. The final design was kept relatively simple so that it could be printed quickly while still meeting the requirement of attaching securely to the artifact.

---

# 3D Printing Documentation

## STL and PrusaSlicer Setup

After completing the SolidWorks model, I exported the part as an STL file and opened it in PrusaSlicer. I positioned the part with its large flat bottom surface against the build plate. This orientation gave the component a stable base and allowed most of the geometry to print without requiring additional support material.

---

## Print Size and Build Volume

The final sliced component measured approximately **31.83 mm × 16.90 mm × 7.90 mm**. These dimensions were larger than the original artifact because the printed component included the outside walls and supporting material surrounding the mating feature.

The final design was still small enough to print quickly and required only a small amount of PLA.

<img width="2048" height="1080" alt="Unknown-11" src="https://github.com/user-attachments/assets/f3c8979e-f18c-4b71-8a45-cb6b68fc7aad" />

---

## Printer and Material

I prepared the part using a **Prusa CORE One with a 0.4 mm nozzle**. The material selected in PrusaSlicer was **Generic PLA** with a filament diameter of **1.75 mm**.

The PLA nozzle temperature was set to **230°C for the first layer** and **220°C for the remaining layers**. The bed temperature was set to **60°C**.

<img width="585" height="302" alt="Unknown-9" src="https://github.com/user-attachments/assets/fafd1033-0e01-45e4-80cf-6dc08ff09732" />


---

## Layer and Wall Settings

The layer height was set to **0.20 mm**, and the first layer height was also set to **0.20 mm**. The model used two vertical perimeters. The top surfaces used five solid layers, while the bottom used three solid layers.

I used these settings because the part was small and did not require an extremely fine layer height. A 0.20 mm layer height provided enough detail for the snap features while keeping the printing time low.

<img width="725" height="622" alt="Unknown-6" src="https://github.com/user-attachments/assets/0c893937-7f0b-49f4-94cb-c0323827d578" />


---

## Infill Settings

The infill density was set to **15%** using a **Grid** infill pattern. The infill angle was set to 45 degrees.

I chose 15% infill because the component is small and most of its strength comes from its outside walls and overall geometry. A higher infill percentage would have increased printing time and material use without being necessary for this design.

<img width="557" height="474" alt="Unknown-7" src="https://github.com/user-attachments/assets/4ab3d595-c764-43f3-b1b9-c5a48376c686" />


---

## Supports and Build Orientation

The final sliced model was printed with **no supports**. I selected this orientation because the large bottom surface could sit directly on the build plate and most of the angled geometry could be printed without separate support structures.

Avoiding supports also reduced material use and eliminated the need to remove support material after printing. The thicker outside walls that I added near the end of the design process also helped give the component more support and stability in the sliced model.

<img width="534" height="527" alt="Unknown-8" src="https://github.com/user-attachments/assets/dd41e92b-c338-4ae3-8673-6769c154cd6d" />


---

## Final Sliced Model

After slicing, PrusaSlicer showed that the model used approximately **39 layers**, with the final height reaching approximately **7.80 mm** in the layer preview. The estimated total printing time was approximately **7 minutes**.

The slicer preview allowed me to check the walls, infill, snap features, and individual layers before sending the file to the printer. This was important because I could confirm that the added outside thickness was actually being printed as intended.


---

## Printing Process

After checking the sliced model, I transferred the print file to the 3D printer. I monitored the beginning of the print to make sure that the first layer attached correctly to the build plate and that the model printed in the intended orientation.

I also recorded a short video of the component during the printing process as required for the lab documentation.

<img width="320" height="568" alt="Lab 6" src="https://github.com/user-attachments/assets/0f05e1dc-9973-4d3a-a69e-61c31db7768b" />



---

# Fit Testing

## Testing the Printed Component

After the print was completed, I tested the component directly on the original artifact. The purpose of the test was to determine whether the measured dimensions, 0.30 mm clearance, and snap features allowed the artifact to fit securely inside the printed part.

The snap features were designed so that the artifact could be pushed into the component using hand pressure. Once the artifact passed the angled portion of the snaps, the features were intended to help hold it in position so that it could not be pulled apart easily.

<img width="232" height="197" alt="Screenshot 2026-09-29 at 1 50 23 PM" src="https://github.com/user-attachments/assets/27a43b7b-6d99-46b6-bdd6-c46a6ac4b531" />


---

## Final Fit

The final fit was tested by attaching the printed component to the artifact and checking whether the snap features held the two pieces together.

<img width="342" height="229" alt="Screenshot 2026-09-29 at 1 50 07 PM" src="https://github.com/user-attachments/assets/9b58e15c-5a76-48d6-86ec-d2808c39317e" />

If the fit required an additional adjustment, the dimensions controlling the clearance or snap geometry could be changed in SolidWorks without rebuilding the entire model because the design was created parametrically.

---

# Show and Tell

The completed component was designed specifically to fit the measured artifact. The final design uses two matching snap features to secure the artifact inside the printed component. This is a quick video of me trying to pull the part off the design. 

<img width="320" height="180" alt="Lab 6 Show and Tell" src="https://github.com/user-attachments/assets/8f64cf9b-6519-428b-9576-a2ec598787c9" />


---

# Lessons Learned

This project showed me how important accurate measurements are when designing a CAD model that must interact with a real object. A dimension that is only slightly incorrect can prevent a printed part from fitting correctly. I also learned why clearance must be considered instead of simply using the exact measured dimensions of the artifact.

Another important lesson was considering how the CAD model would actually behave when it was 3D printed. During the design process, I decided that the outside portions of my original model were too thin. I increased the outside thickness to give the component better support and make it stronger when sliced and printed. This was an important change because the design needed to be strong enough to withstand the force of inserting and removing the artifact.

I also learned that the orientation of a model can affect how much support material is required. By placing the large flat surface against the build plate, I was able to slice the final design without supports. This reduced material usage, reduced cleanup after printing, and kept the estimated print time to approximately seven minutes.

Using dimensions, constraints, and mirrored features in SolidWorks also made the model easier to control. Instead of independently creating every feature, I was able to create one side and mirror matching geometry to the opposite side. This helped keep the final design symmetrical.

---

# Time and Resources

I used calipers to measure the artifact, graph paper to create the initial hand sketch, SolidWorks to create the parametric CAD model, PrusaSlicer to prepare the STL file, PLA filament for the final component, and a Prusa CORE One 3D printer with a 0.4 mm nozzle.

The estimated printing time shown by PrusaSlicer was approximately **7 minutes**.

**Measurement and Hand Sketch Time:** 45 minuets 

**SolidWorks Design Time:** 2 hours

**Slicing and Setup Time:** 20 minuets

**Printing Time:** 15 minuets

**Fit Testing Time:** 5 mintues

**Total Project Time:** 3 hours and 30 minutes  

