# LAB 5 - Design a Snap Fit

## Hand Calculations

The goal of this project was to design a two-component snap-fit assembly that could be modeled parametrically, 3D printed, and assembled using elastic deformation. PLA was selected as the material. A safety factor of 3.5 was used as required, with a transverse design load of 0.25 lbf and an axial clip load of 5 lbf.

The main box dimensions used in the design were 60 mm long, 40 mm wide, and initially extruded 10 mm. The wall thickness was set to 2 mm. The snap feature was modeled with an 18 mm length, 2 mm height, and 10 mm extrusion. A 45° angled surface was used on the snap to help the lid slide into position during assembly.

<img width="574" height="724" alt="Screenshot 2026-09-22 at 12 46 50 PM" src="https://github.com/user-attachments/assets/be2449ef-eb0b-4478-9459-31f58e32f04d" />


<img width="603" height="862" alt="Screenshot 2026-09-22 at 12 46 33 PM" src="https://github.com/user-attachments/assets/586555bd-914a-46ee-8f4b-bdc47776eb64" />


<img width="537" height="721" alt="Screenshot 2026-09-22 at 12 47 13 PM" src="https://github.com/user-attachments/assets/fa293aba-ba9e-4330-ad97-2b724507734a" />

---

## SolidWorks Design

The snap-fit box was modeled in SolidWorks using MMGS units. The initial base sketch was a centered rectangle measuring 60 mm by 40 mm. This sketch was extruded 10 mm to create the starting solid.



<img width="1289" height="659" alt="Screenshot 2026-09-22 at 12 20 35 PM" src="https://github.com/user-attachments/assets/7b550cc8-273a-4c94-9c4f-be2172f11ff3" />



<img width="1298" height="672" alt="Screenshot 2026-09-22 at 12 20 46 PM" src="https://github.com/user-attachments/assets/c7263caa-231f-48f9-8d12-29f6d45d708c" />


A 10 mm radius fillet was applied to the four corners to create the rounded rectangular shape. The model was then shelled using a 2 mm wall thickness. The rounded geometry removed sharp exterior corners while the 2 mm shell created the box walls.



<img width="1344" height="634" alt="Screenshot 2026-09-22 at 12 20 57 PM" src="https://github.com/user-attachments/assets/c14c6eee-cb03-4549-86f3-7e4018653f78" />



<img width="1276" height="682" alt="Screenshot 2026-09-22 at 12 21 08 PM" src="https://github.com/user-attachments/assets/a8a3e30e-e803-4516-81b8-1b6905211532" />



A 0.20 mm offset was used between mating geometry to provide an engineered allowance between the lid and the box. This clearance was added because an exact zero-clearance fit would make the printed components difficult to assemble due to normal FDM printing tolerances.



<img width="1240" height="600" alt="Screenshot 2026-09-22 at 12 21 22 PM" src="https://github.com/user-attachments/assets/59e2b5d5-714e-42aa-824b-607dfd83a254" />


The snap feature was modeled at 18 mm long and 2 mm high and was extruded 10 mm. A 45° angled surface was added to the snap so that the mating part could slide over the feature rather than contacting a vertical face directly. A 1 mm chamfer was also added where appropriate to reduce sharp edges and make assembly easier.



<img width="1393" height="675" alt="Screenshot 2026-09-22 at 12 21 52 PM" src="https://github.com/user-attachments/assets/7dc0fe7b-563f-4418-8387-e730091db6a7" />


<img width="1234" height="690" alt="Screenshot 2026-09-22 at 12 22 03 PM" src="https://github.com/user-attachments/assets/73e0ece6-40ec-4504-9428-c837ed12bd0c" />


<img width="1280" height="630" alt="Screenshot 2026-09-22 at 12 22 22 PM" src="https://github.com/user-attachments/assets/c9ebcd50-f6c0-43da-a689-8e54d15126de" />


Mirror features were used to reproduce the snap geometry on the opposite side of the box. Using the mirror command ensured that both snap locations remained symmetric instead of manually recreating the feature and risking dimensional differences.



<img width="1380" height="634" alt="Screenshot 2026-09-22 at 12 22 47 PM" src="https://github.com/user-attachments/assets/6c5fe47d-e81b-43ff-94d7-9e2dd692ce9d" />


The side profile was used to check how the lid and base fit together and to verify the snap geometry from the side.

### Parametric Design

The main parameters used in the design were the overall box length and width, extrusion height, wall thickness, corner radius, lid clearance, snap dimensions, and snap angle. These parameters were chosen because they directly control the size of the box, the fit between the two components, and the geometry of the snap connection.

The important values used were 60 mm for the box length, 40 mm for the width, 10 mm for the initial extrusion, 10 mm for the corner radius, 2 mm for the wall thickness, 0.20 mm for the lid clearance, 18 mm for the snap length, 2 mm for the snap height, and 45° for the snap ramp.

The dimensions were kept consistent during the final modeling process once the overall geometry was established. Mirror features were used where possible so that repeated geometry remained controlled by the original feature instead of being dimensioned independently.

The engineered allowance between the interactive parts was primarily controlled by the 0.20 mm offset. This clearance was selected to prevent the lid and base from being modeled at exactly the same size while still keeping the fit relatively tight after printing.



<img width="1269" height="647" alt="Screenshot 2026-09-22 at 12 23 00 PM" src="https://github.com/user-attachments/assets/1d977e55-5a45-44df-8f45-e0728d4ed125" />

---

## PLA Material

PLA was selected as the printing material because it is commonly used for FDM printing and is suitable for a small snap-fit prototype. The SolidWorks model was assigned PLA material properties so that the material selection was documented with the CAD model.

The calculated design values were compared with the strength of PLA using the required safety factor. The snap feature was designed so that the calculated stresses remained below the selected allowable stress.

The completed SolidWorks base had a calculated mass of approximately 11.22 g, a volume of 9044.67 mm³, and a surface area of 9599.12 mm².



<img width="1310" height="663" alt="Screenshot 2026-09-22 at 12 23 11 PM" src="https://github.com/user-attachments/assets/5b51204b-af15-4008-a2d5-0a26f0a58e18" />

---

## Build Orientation Research

FDM printed parts do not have equal strength in every direction because the part is built one layer at a time. The bond between layers in the Z direction is generally weaker than loading within the printed layers. For a part subjected to bending, the flexing region should therefore be oriented so that the primary load acts along the printed layers rather than attempting to separate them. UltiMaker similarly recommends considering model orientation for functional FDM parts because parts are often weaker in the Z direction. :contentReference[oaicite:0]{index=0}

For this design, the components were placed flat on the build plate so that the main geometry and snap features could be produced with the layers running through the body of the part. This orientation also provided a large contact area with the print bed and helped keep the parts stable during printing.

Research source: UltiMaker, *How to Design for FFF 3D Printing*.

---

## PrusaSlicer Setup

The two components were imported into PrusaSlicer and positioned flat on the build plate. Both parts were placed close to the center of the build area while leaving enough space between them for printing.



<img width="1357" height="717" alt="Screenshot 2026-09-22 at 12 23 53 PM" src="https://github.com/user-attachments/assets/a8a3d8a3-8e23-45cb-8145-873356f9f765" />



Generic PLA was selected as the filament. The printer profile used a 0.4 mm nozzle with a 0.20 mm layer height. The first layer height was also set to 0.20 mm.

The model used two perimeters with five top solid layers and three bottom solid layers. These settings provided a balance between print time and having enough exterior material around the snap-fit components.



<img width="965" height="671" alt="Screenshot 2026-09-22 at 12 24 04 PM" src="https://github.com/user-attachments/assets/0b0062f8-ea1b-4643-8498-949fde00a3a6" />



The infill density was set to 15% with a Grid infill pattern. The design uses relatively thin walls and exterior shells, so the walls and perimeters provide much of the structure while the 15% infill reduces unnecessary material and printing time.



<img width="731" height="257" alt="Screenshot 2026-09-22 at 12 24 27 PM" src="https://github.com/user-attachments/assets/46319f22-f4b2-4528-a903-462a860e88ce" />



The PLA filament diameter was 1.75 mm. The first-layer nozzle temperature was set to 230°C and the nozzle temperature for the remaining layers was 220°C. The build plate temperature was set to 60°C.



<img width="724" height="342" alt="Screenshot 2026-09-22 at 12 24 35 PM" src="https://github.com/user-attachments/assets/acdd9207-f484-4200-9787-26587cb11759" />


The slicer estimated a total print time of approximately 28 minutes in normal mode. The two parts used approximately 17.83 g of filament based on the slicer estimate.

Supports were not used in the slicer setup shown. The parts were oriented so that most geometry could be produced directly from the build plate without unnecessary support material. If support material is required for the final assignment demonstration, support can be added only to the area that needs it rather than supporting the entire model.

---

## Printing and Snap-Fit Test

After printing, the base and lid were inspected separately before assembly. The 0.20 mm mating clearance was intended to allow the lid to fit over the base without requiring an exact interference fit. Before printing, I changed the filament loaded in the printer to PLA so it matched the material selected in PrusaSlicer. The printer used was the **Prusa CORE ONE PL_05**, matching the printer name provided on the thumb drive. I then confirmed the PLA settings, sliced both components, and exported the finished print file.

<img width="347" height="337" alt="Screenshot 2026-09-22 at 12 50 49 PM" src="https://github.com/user-attachments/assets/8fb6afdb-11ef-4393-b63b-da63c1a34716" />


The lid was then installed onto the base and the snap-fit connection was tested. The angled snap geometry allowed the mating surfaces to slide past each other before engaging.

<img width="351" height="287" alt="Screenshot 2026-09-22 at 12 50 58 PM" src="https://github.com/user-attachments/assets/00d39424-3880-4454-8813-8604f6b7f377" />


A short video was recorded to demonstrate the snap-fit assembly being installed and/or removed. This provides evidence that the two printed components physically fit together and demonstrates the elastic snap-fit behavior required by the assignment.

<img width="202" height="360" alt="Lab 5 GIF" src="https://github.com/user-attachments/assets/daf2a9e3-d7ee-4ac7-b78b-419d93914c28" />


---

## Mistakes, Changes, and Lessons Learned

### Lessons Learned

One of the most important parts of the design was maintaining enough clearance between the lid and base. The 0.20 mm offset was used because printed components cannot be expected to fit properly if the CAD surfaces are modeled directly on top of each other. Using Mirror in SolidWorks was also useful because the same snap feature was required on both sides. Instead of independently recreating the second snap, mirroring the original feature kept the design symmetric and reduced the possibility of introducing a different dimension on the opposite side. The project also demonstrated that print orientation has to be considered as part of the mechanical design rather than only as a slicer setting. Because FDM parts are built in layers, the orientation of a flexible feature can affect whether it bends through the material or separates between layers. This was considered when laying out the parts for printing. The final design combined the hand calculations, parametric SolidWorks model, engineered clearance, mirrored snap geometry, and PrusaSlicer settings into a two-component snap-fit box that could be physically assembled and tested. Engineering is always about finding innovative ways to make our lives easier and to find the most effective way to carry out a step. 

### Mistakes

After completing the part I realized that I needed to find a way to export the STL files in their two separate bodies rather than the whole thing, I soon learned that after doing my first export. Exporting them as one body would not only call for me to add supports but it defeats the purpose of this task. I went back into solid works and carried out the following steps to export the body parts separately:

Insert --> Features --> Save bodies... 

I then selected the Lid; saved that as its own .sldprt file and likewise with the Body. After that I then saved it as an STL file and that that imported into PrusaSlicer. 

### Changes

One change I had to make was switching the printer filament setting to PLA so the slicer matched the material actually being used. This made sure the temperature and print settings were appropriate for the final part.
