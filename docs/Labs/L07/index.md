# Slider-Crank Mechanism

## Introduction

For this project, I designed and 3D printed a slider-crank mechanism. The purpose of the mechanism is to convert rotational motion into back-and-forth linear motion. I created each component separately in SolidWorks, assembled the parts using mates, exported the parts as STL files, and prepared them for printing in PrusaSlicer.

---

# 1. Research

## Variable-Stroke Slider-Crank Mechanism

One mechanism I researched was a variable-stroke slider-crank mechanism used in an internal combustion engine. A standard slider-crank converts the rotational motion of a crankshaft into the back-and-forth linear motion of a piston. In this design, additional linkage is used to change the piston stroke and compression ratio. This type of mechanism can be used in the automotive industry for engine systems. Similar slider-crank mechanisms are also used in power equipment such as generators, pumps, and other machines that use piston movement. This mechanism relates closely to my project because my design also uses a crank and connecting link to convert rotational motion into linear movement.

<img width="778" height="459" alt="Screenshot 2026-10-06 at 11 37 02 AM" src="https://github.com/user-attachments/assets/a3f0f247-1cc3-4414-a678-fce96acb003a" />


*Figure 1. Variable-stroke slider-crank mechanism. Source: SAE International, 2021.*

---

## Four-Bar Linkage Robotic Arm

The second mechanism I researched was a four-bar linkage used in a robotic manipulator arm. A four-bar linkage uses several rigid links connected by rotating joints. When one link moves, the other links follow a controlled path. This type of mechanism can be used in manufacturing for robotic pick-and-place systems. It can also be used in automation and packaging where products or tools need to move repeatedly along a controlled path. This mechanism is similar to my slider-crank because both designs use rigid links and pivot joints to transfer motion from one component to another.


<img width="228" height="189" alt="Screenshot 2026-10-06 at 11 44 46 AM" src="https://github.com/user-attachments/assets/c001aadc-420c-466c-a787-500af13fe305" />


*Figure 2. Four-bar linkage robotic arm. Source: Zomerdijk and van der Wijk, 2022.*

---

## Connection to My Design

After researching these mechanisms, I chose to build a slider-crank mechanism. My design uses a support, a short crank link, a long connecting link, a slider, a guideway, and pivot pins. As the crank rotates, the long connecting link pushes and pulls the slider through the guideway.

The research helped me understand how linkage systems are used to control movement and how rotational motion can be converted into linear motion.

---

## Research Sources

1. Henao Castañeda, E. J., Romero, C. A., & Quintero, H. F.  
   "Development Work on the Synthesis of a Variable Stroke Slider-Crank Mechanism for a Variable Compression Ratio Combustion Engine."  
   SAE International, 2021.

2. Zomerdijk, M. J. J., & van der Wijk, V.  
   "Structural Design and Experiments of a Dynamically Balanced Inverted Four-Bar Linkage as Manipulator Arm for High Acceleration Applications."  
   *Actuators*, 2022.

3. Yao, X., Wang, X., Sun, W., Kong, J., & Lin, Z.  
   "Optimal Synthesis of Four-Bar Linkages for Path Generation Using the Individual Repairing Method."  
   *Mechanical Sciences*, 2022.

---

# 2. Design

## Purpose

The purpose of my mechanism is to convert rotational motion into linear motion. I chose a slider-crank because it clearly shows how several connected parts can transfer motion through rotating and sliding joints. It was also simple enough to model and print while still including multiple moving interfaces.

---

## Components

| Component | Function | Type |
|---|---|---|
| Support | Holds the main fixed pivot | 3D Printed |
| Link 2 / Short Crank Link | Transfers rotation from the support to the long link | 3D Printed |
| Long Connecting Link | Transfers motion to the slider | 3D Printed |
| Slider | Moves back and forth | 3D Printed |
| Guideway | Keeps the slider moving in a straight path | 3D Printed |
| Pivot Pins | Connect the moving parts | 3D Printed |
| Cap | Keeps the Link 2 connection from slipping off the pivot | 3D Printed |

---

# Individual Part Design

## Support

I started by sketching the support profile in SolidWorks. The bottom section was made wider to provide a stable base, while the top section was rounded around the main pivot location. I extruded the sketch to create the main body and then added the cylindrical pivot that connects to Link 2.

The support provides the fixed pivot point for the mechanism.

<img width="449" height="541" alt="Unknown-1" src="https://github.com/user-attachments/assets/512dcad9-b6de-4461-bd8c-4637617c63bd" />

<img width="862" height="531" alt="Unknown-2" src="https://github.com/user-attachments/assets/8c325d28-8cbd-408e-9319-23cb6f6e0c44" />


<img width="833" height="476" alt="Unknown-3" src="https://github.com/user-attachments/assets/4542d70e-173d-4092-9fba-ee51884da0fd" />


<img width="2048" height="1143" alt="Unknown" src="https://github.com/user-attachments/assets/e921d6f4-c17d-4ef4-9687-51335f6856ae" />





---

## Long Connecting Link

I created the long connecting link using two rounded ends connected by straight lines. The part was designed to be 30 mm wide with a 200 mm center-to-center distance between the holes. After fully defining the sketch, I extruded it to create the final part.

The long connecting link transfers the motion from Link 2 to the slider.

<img width="2048" height="763" alt="Unknown-4" src="https://github.com/user-attachments/assets/b66057ee-1eb5-4b2d-bff7-beeedbe30808" />


<img width="2048" height="831" alt="Unknown-5" src="https://github.com/user-attachments/assets/4c1c2824-3479-4ed7-b234-75d9ab75dcc2" />


---

## Link 2 / Short Crank Link

The short crank link was created using the same basic shape as the long connecting link. It was designed to be 30 mm wide with a 50 mm center-to-center distance between the two holes. I then extruded the profile to create the finished link.

The purpose of Link 2 is to rotate around the support pivot and transfer motion to the long connecting link.

Later, after testing the printed parts, I modified the **left opening on Link 2 to 23 mm in diameter**. The original opening was too tight for the fit I needed, so increasing the diameter gave the joint more clearance.


<img width="898" height="557" alt="Unknown-6" src="https://github.com/user-attachments/assets/72b7b7a0-5ac7-4095-b35b-98a2b843e540" />



<img width="1023" height="500" alt="Unknown-7" src="https://github.com/user-attachments/assets/61334b56-1d26-4bf6-b6d2-5731e549514b" />



---

## Slider

The slider started as a 40 mm by 40 mm rectangular sketch. I extruded the rectangle to create the main slider body and then added a cylindrical pivot to the front face.

The slider connects to the long connecting link and moves back and forth inside the guideway.

<img width="2048" height="1197" alt="Unknown-8" src="https://github.com/user-attachments/assets/7ff64e03-409d-48b5-85a3-6c4d06b05c73" />



<img width="2048" height="1257" alt="Unknown-9" src="https://github.com/user-attachments/assets/d235a0b7-2342-4a67-b7d9-0676b9911341" />


<img width="2048" height="1241" alt="Unknown-10" src="https://github.com/user-attachments/assets/e7724651-7db1-49db-a9eb-a763d0b3211f" />



---

## Guideway

I designed the guideway by creating a side profile with an upper and lower section surrounding the slider. I then extruded the profile to create the full guideway.

The guideway keeps the slider aligned and prevents it from rotating while it moves back and forth.

<img width="771" height="758" alt="Unknown-11" src="https://github.com/user-attachments/assets/d43c0138-d953-448d-b9cf-3a52531466aa" />


<img width="2048" height="1013" alt="Unknown-12" src="https://github.com/user-attachments/assets/4fcd977e-6cf1-4f52-bfe6-4d51db8d567a" />


---

## Pivot Pin

The pivot pin was originally created as a simple cylinder. The pins are used to connect the moving parts and allow the links to rotate.

After importing the first version into PrusaSlicer, I received a low bed adhesion warning because the cylindrical pin had very little contact area with the print bed. I returned to SolidWorks and added a wider circular base to the pin so it would have more surface area touching the bed.

<img width="2048" height="1166" alt="Unknown-13" src="https://github.com/user-attachments/assets/15a5875e-a245-4aef-8eb3-62bca2b23ee0" />


<img width="2048" height="1270" alt="Unknown-14" src="https://github.com/user-attachments/assets/94ffa99d-b8d4-4ca7-b3b0-d7553732db68" />



---

## Cap

After the first print and assembly test, I noticed that one of the connections on Link 2 could slip off the pivot. To fix this, I created a small cap that could be placed over the end of the connection.

The cap helps keep Link 2 in place while still allowing the joint to rotate.

<img width="458" height="414" alt="Screenshot 2026-10-06 at 1 02 11 PM" src="https://github.com/user-attachments/assets/b5e84322-c22f-4829-81c5-7d14baf1b1d6" />

---

# Design Decisions

## Slider-Crank Mechanism

I chose a slider-crank mechanism because the motion is easy to see and understand. It also allowed me to work with both rotating joints and a sliding component in one design.

## Separate Parts

I designed each component as a separate SolidWorks part. This made it easier to change individual pieces without rebuilding the entire mechanism.

## Guideway

I added a guideway around the slider so that the slider would stay aligned and move only in one direction. Without the guideway, the slider could rotate or move out of position.

## Pin Base

I added a wider base to the pivot pin after PrusaSlicer showed a low bed adhesion warning. The larger base gave the pin more contact area with the print bed and improved its stability during printing.

## Larger Link 2 Opening

After the first print, I found that one of the openings on Link 2 needed more clearance. I increased the **left opening to 23 mm in diameter** so the connection could move more freely.

## Cap

I added a cap after noticing that the Link 2 connection could slip off the pivot. The cap keeps the link in place while still allowing the joint to move.

---

# CAD Development

The following images show the main stages of the SolidWorks design process.

**CAD Stage 1 – Support**


<img width="2048" height="1143" alt="Unknown" src="https://github.com/user-attachments/assets/922f0515-2d9a-4e26-940c-e19e81027560" />


**CAD Stage 2 – Long Connecting Link**

<img width="2048" height="831" alt="Unknown-5" src="https://github.com/user-attachments/assets/5dcfb7d0-786b-4473-b0e4-0c6d4efdd256" />


**CAD Stage 3 – Link 2**


<img width="1023" height="500" alt="Unknown-7" src="https://github.com/user-attachments/assets/14d92b94-8359-4302-85cb-d97104dc194f" />


**CAD Stage 4 – Slider**


<img width="2048" height="1241" alt="Unknown-10" src="https://github.com/user-attachments/assets/c39b0823-874d-4412-96d1-be17df4911bf" />


**CAD Stage 5 – Guideway**

<img width="437" height="459" alt="Screenshot 2026-10-06 at 1 04 04 PM" src="https://github.com/user-attachments/assets/8a4181ad-0775-4327-bbe4-1e1322076b27" />


**CAD Stage 6 – Pivot Pin**

<img width="2048" height="1071" alt="Unknown-19" src="https://github.com/user-attachments/assets/3701f296-98d4-4292-9917-add15700cb42" />


**CAD Stage 7 – Cap / Link 2 Revision**

<img width="473" height="458" alt="Screenshot 2026-10-06 at 1 04 29 PM" src="https://github.com/user-attachments/assets/b29a7ea8-1035-49e7-872a-dce126984079" />


---

# SolidWorks Assembly

After finishing the individual parts, I created a SolidWorks assembly and inserted the support, Link 2, long connecting link, slider, guideway, and pins. I used concentric, coincident, and distance mates to line up the pivot points and position the components correctly. The mates allowed the rotating parts to move around the pins while keeping the slider aligned with the guideway. The completed assembly showed how Link 2 transfers rotation into motion of the long connecting link, which then moves the slider back and forth.

<img width="2048" height="1124" alt="Unknown-16" src="https://github.com/user-attachments/assets/3caf21d8-91ce-4fc6-81cd-c2b1cf82b04c" />


---

# 3. 3D Printing

## Exporting the Parts

After completing the SolidWorks assembly, I exported the individual components as STL files and imported them into PrusaSlicer.

**Insert Image Here**

<img width="2048" height="1022" alt="Unknown-17" src="https://github.com/user-attachments/assets/49529bcd-e954-443c-b9c9-cf1dc80d16a4" />





---

## Scaling the Model

After importing the STL files, I decided to scale every component down to **50% of the original size**. The original model was larger than necessary and would have taken longer to print.

Scaling all parts by the same amount kept the mechanism proportional while reducing the overall print time and material use.

<img width="2048" height="1089" alt="Unknown-20" src="https://github.com/user-attachments/assets/3bd066c0-3863-4fda-aa32-27ab700f1aa2" />


---

## First Pin Modification

During the first slicing attempt, PrusaSlicer showed a low bed adhesion warning for the original pivot pin. The original cylinder had a small amount of surface area touching the build plate.

I returned to SolidWorks and added a wider circular base to the bottom of the pin. I then exported the updated STL and replaced the original part in PrusaSlicer.

<img width="879" height="372" alt="Unknown-18" src="https://github.com/user-attachments/assets/6e67c659-a181-4a99-9c1d-36ababbed4d5" />

<img width="2048" height="1071" alt="Unknown-19" src="https://github.com/user-attachments/assets/62791fd0-b78c-4bfe-9a6e-7b5398efa9bc" />


---

## First Print

After making the pin change, I arranged the parts on the build plate and prepared the first complete print.

The first print allowed me to check how the actual parts fit together instead of only relying on the SolidWorks assembly.

<img width="426" height="399" alt="Screenshot 2026-10-06 at 1 06 22 PM" src="https://github.com/user-attachments/assets/e6825c00-10ec-4415-b8fc-ceca88dc417b" />

---

## Second Print and Fit Adjustment

After testing the first printed parts, I found that one connection on Link 2 needed to be changed. I increased the **left opening on Link 2 to 23 mm in diameter** so the joint would have more clearance.

I also designed and added a **cap** because the connection could slip off the pivot during movement. The cap keeps the link in position while still allowing the joint to rotate.

I exported the revised Link 2 and the new cap as STL files and prepared them for a second print in PrusaSlicer.

**Insert Second Print Slicer Image Here**

![Second Print - Link 2 and Cap](INSERT-IMAGE-HERE)

---

# Print Settings

The main parts were prepared for printing on printer **PC-12**.

| Setting | Value |
|---|---|
| Printer | PC-12 |
| Material | PETG |
| Nozzle | 0.4 mm |
| Layer Height | 0.20 mm |
| First Layer Height | 0.20 mm |
| Perimeters | 2 |
| Top Solid Layers | 5 |
| Bottom Solid Layers | 3 |
| Infill | 15% |
| Infill Pattern | Grid |
| Nozzle Temperature | 240°C |
| Bed Temperature | 85°C |
| Supports | None |
| Scale | 50% |
| Estimated First Print Time | About 55 minutes |
| Estimated First Print Material | About 25.79 g |

For the second print, only the revised Link 2 and cap were printed.


<img width="581" height="559" alt="Unknown-21" src="https://github.com/user-attachments/assets/b7c11dcc-1368-4686-8cfc-0459a74aa545" />


<img width="449" height="359" alt="Unknown-22" src="https://github.com/user-attachments/assets/e8997c2a-d9ff-4209-bdaf-1deb90335daa" />


<img width="487" height="291" alt="Unknown-23" src="https://github.com/user-attachments/assets/97a12fc3-5a07-42c2-b23b-70191cefe856" />



---

# Printing Process

The components were printed using the PC-12 printer. I monitored the print to make sure the parts stayed attached to the build plate and that the redesigned pin printed correctly. After the first print finished, I removed the components from the build plate and checked the fit of the pivot connections and the slider. This fit check is what led to the second print. I found that Link 2 needed more clearance and that a cap would help keep the connection from slipping off. After printing the revised Link 2 and cap, I tested the fit again before completing the final assembly.



---

# Final Assembly

After checking all of the printed components, I assembled the complete slider-crank mechanism.

The short crank rotates around the fixed support pivot and moves the long connecting link. The long link then pushes and pulls the slider through the guideway. The revised 23 mm opening on Link 2 allows the joint to move more freely, while the added cap helps keep the connection from slipping off.

The completed mechanism converts rotational motion into back-and-forth linear motion.



<img width="426" height="399" alt="Screenshot 2026-10-06 at 1 06 22 PM" src="https://github.com/user-attachments/assets/f6e3e020-09fc-46a3-b20a-c5b8cbc12fcf" />




<img width="180" height="320" alt="ezgif com-video-to-gif-converter" src="https://github.com/user-attachments/assets/e06bcad7-4988-4abf-86c7-5dee315686e9" />


---

# 4. Lessons Learned

## Time

I spent approximately:

- 2 hours researching
- 4 hours creating the SolidWorks parts
- 1 hour building and adjusting the assembly
- 30 mins preparing the STL files and PrusaSlicer setup
- **About 55 minutes** on the first print
- **About 5 minutes** on the revised Link 2 and cap print
- *1 hour assembling and testing the mechanism

The project took about 8 hours in total. 

---

## Biggest Mistake

The biggest issue I ran into was assuming that the original CAD fit would work exactly the same after printing. During testing, I found that one of the Link 2 connections was too tight and that the link could also slip off the pivot. I fixed these problems by increasing the left opening on Link 2 to **23 mm in diameter** and by designing a cap to hold the connection in place. The second print allowed me to correct both issues without having to print the entire mechanism again. In the end the project was not a success. Even after my final second print the parts did not do the correct function and that is moving the slicer in a linear motion. The biggest take away was that I needed to build and dimension my components in respect to how it will function after it has been printed rather than only worrying about it fitting tightly on the assembly in solid works. 

---

## Tolerances

The first-print clearances did not work perfectly at every connection. One of the openings on Link 2 was too tight, so I increased the left opening to **23 mm in diameter**. The slider and the other pivot connections could be checked during assembly, while the Link 2 connection required the main adjustment. If I printed the mechanism again, I would include slightly more clearance in the moving joints from the beginning so the parts could rotate more freely without requiring a second print. The main moving interfaces in the mechanism are the pivot connections and the slider inside the guideway. These joints need clearance so the parts can move without becoming too tight. The original CAD model used nominal dimensions around 20 mm for the pivot areas. After the first print, I found that one connection on Link 2 needed more clearance. I changed the **left opening on Link 2 to 23 mm in diameter**. This change gave the joint more room to rotate and made assembly easier. The slider also requires clearance inside the guideway so it can move back and forth without binding. Because I later scaled the complete model to 50% in PrusaSlicer, all original CAD dimensions and clearances were also reduced by half in the printed version.

