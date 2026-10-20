# Functional 3D Printing Project – Desk Organizer

## 1. Reading and Writing – Design Thinking 

After reading Great Questions Lead to Great Design: A Guide to the Design-thinking Process, I learned that asking the right questions is important when designing something. It helps identify the problem, understand what the user needs, and find a practical solution. During my project, I realized that my original idea would take too long to print, so I adjusted the size and found another useful purpose for it. This showed me that making changes throughout the design process can lead to a better final product.

## 2. Problem Statement 

My original idea was to design a sock holder for my closet to keep my socks organized. However, after creating the model in SolidWorks, I realized that printing it at its original size would take over 15 hours. Instead of starting over, I decided to scale the model down and turn it into a desk organizer. I plan to use it to hold my keys, AirPods, small cologne, and other small belongings so that my desk stays cleaner. I spent about one hour deciding what I wanted to create and researching ideas for a functional design. I wanted something simple, practical, and easy to print. Although I designed it for myself, it could also be useful for students or anyone who wants to organize smaller items on their desk.

## 3. Design Process – SolidWorks 

### Step 1: Creating the Base

I started by creating a rectangular sketch in SolidWorks. Using Smart Dimension, I set the base to 8 inches long and 6 inches wide. I did not make any paper sketches because I completed the entire design directly in SolidWorks.

**Figure 1 – Initial SolidWorks sketch**

<img width="2048" height="1019" alt="Unknown" src="https://github.com/user-attachments/assets/5b04c688-3aa5-4c48-b418-fed156526342" />


### Step 2: Extruding the Main Body

I used Boss-Extrude to create the main body of the organizer. I initially extruded the rectangular sketch to a height of 5 inches. This gave me the main shape that I could modify into a storage container.

**Figure 2 – Boss-Extrude of the main body**

<img width="2048" height="966" alt="Unknown-1" src="https://github.com/user-attachments/assets/4b6d8e3d-343e-4a3b-812f-895b37783425" />


### Step 3: Creating the Front Opening

Next, I used Cut-Extrude to remove material and create an opening at the front. I used the Up to Surface option and included a 2-inch dimension in the opening. This would make it easier to reach inside the organizer and grab smaller belongings.

**Figure 3 – Creating the front opening**

<img width="2048" height="974" alt="Unknown-2" src="https://github.com/user-attachments/assets/8015cbc0-5578-4f43-9f60-c5449a23d202" />


### Step 4: Adding the Divider

I created an internal divider using Boss-Extrude to separate the organizer into two compartments. I then used Cut-Extrude to slope the divider toward the front. I wanted the compartments to be separate while keeping the front accessible.

**Figure 4 – Creating the center divider**

<img width="959" height="543" alt="Unknown-3" src="https://github.com/user-attachments/assets/0cedc687-4733-410a-976f-5775a8724de4" />


### Step 5: Final SolidWorks Design

The completed model had two compartments, an open top, and a lowered front section. I kept the design simple because I wanted something functional without additional moving parts. It took me approximately **25 minutes** to complete the design in SolidWorks.

**Figure 5 – Modifying the divider**

<img width="2048" height="1075" alt="Unknown-4" src="https://github.com/user-attachments/assets/37db2189-af2b-4a21-98ba-20e92594a035" />


### Step 6: Scaling Down the Design

After exporting the model as an STL file, I imported it into PrusaSlicer. The original print was going to take over 15 hours, so I decided to reduce the model to **40% of its original size**.


| Dimension | Original | Scaled |
|---|---|---|
| Length | 8 in | 3.2 in |
| Width | 6 in | 2.4 in |
| Height | 7 in | 2.8 in |

This reduced the printing time significantly while still leaving enough space for my smaller desk belongings.

**Figure 6 – Completed SolidWorks model**

<img width="876" height="702" alt="Unknown-5" src="https://github.com/user-attachments/assets/fc55948a-2879-4295-83c3-873c3da8de89" />


**Figure 7 – PrusaSlicer showing the scaled model**

<img width="2048" height="1044" alt="Unknown-6" src="https://github.com/user-attachments/assets/d9dc8cbe-45a3-4316-9420-a52ebcb83611" />


### Design Decisions and Allowances

I chose a rectangular shape because it provides a flat, stable base. I added the divider to separate belongings and lowered the front to improve accessibility. Since the organizer was designed as one piece, I did not need clearances for moving or connecting parts. However, I had to consider that scaling the model down would also reduce the wall thickness. I kept the design intended for lightweight items.

## 4. 3D Printing Process 

### Printer and Print Settings

I used **PC-10** to print my organizer and prepared the model using PrusaSlicer with a Prusa CORE One profile and Generic PETG filament.

| Setting | Value |
|---|---|
| Printer | PC-10 |
| Material | PETG |
| Nozzle diameter | 0.4 mm |
| Layer height | 0.20 mm |
| Perimeters | 2 |
| Infill | No infill intended |
| Supports | None |
| Raft / Brim | None |
| Nozzle temperature | 240°C |
| Bed temperature | 85°C |
| Number of layers | 356 (slicer preview) |

I did not intend to use infill because the organizer was already hollow and designed to hold lightweight objects. I also did not use supports because the design had an open top and mostly vertical walls. The flat base allowed me to position the organizer upright directly on the print bed without a raft or brim. Since there were no supports, I did not need any tools to remove them or deal with rough support-contact surfaces.

**Figure 8 – PrusaSlicer preview and printing information**

<img width="2048" height="1044" alt="Unknown-6" src="https://github.com/user-attachments/assets/570ae864-a927-48ee-b686-6c62f1037dd0" />


**Figure 9 – Layer height and wall settings**

<img width="745" height="747" alt="Unknown-7" src="https://github.com/user-attachments/assets/9c785aba-d96d-4081-8118-97dd34b820f7" />


**Figure 10 – Infill settings**

<img width="769" height="615" alt="Unknown-8" src="https://github.com/user-attachments/assets/d1f78679-9501-4804-88d5-4d7f03834dda" />


**Figure 11 – PETG filament and temperature settings**

<img width="735" height="286" alt="Unknown-9" src="https://github.com/user-attachments/assets/e7201c71-6e55-4a68-89a9-322576083bca" />


### Printing Time and Material Usage

After scaling the model, PrusaSlicer estimated the following:

| Print Information | Estimate |
|---|---|
| Printing time | 1 hour 33 minutes |
| Filament | 55.93 g |
| Material volume | 2.69 in³ |
| Number of layers | 356 |
| Final dimensions | 3.2 × 2.4 × 2.8 in |

The overall bounding-box volume was approximately 21.5 cubic inches, but the actual material volume was much smaller because the organizer was hollow. These estimates came from the slicer preview showing 15% grid infill. The final values would need to be updated if the print was resliced using 0% infill.

### Video of the Printing Process

I recorded the printing process to document how the organizer was manufactured using PC-10.

**Video 1 – 3D printing the desk organizer**

<img width="180" height="320" alt="ezgif com-video-to-gif-converter-2" src="https://github.com/user-attachments/assets/13d3a162-2f43-4478-865e-2d68225c27d1" />




### Final 3D Printed Product

The finished organizer is intended to hold my everyday belongings and help keep my desk organized. Its two compartments allow me to separate smaller items rather than keeping everything in one place.

The surface finish can be evaluated by checking for visible layer lines, rough edges, and any printing defects. Since no supports were used, there are no support-contact surfaces requiring cleanup.

**Figure 12 – Final printed organizer (front view)**

<img width="426" height="414" alt="Screenshot 2026-10-20 at 1 43 03 PM" src="https://github.com/user-attachments/assets/e702b1e3-581e-47db-9343-ede96d6e3d10" />


**Figure 13 – Final printed organizer (top view)**

<img width="616" height="494" alt="Screenshot 2026-10-20 at 1 44 20 PM" src="https://github.com/user-attachments/assets/f09bf952-960f-447a-ac0b-8a282b3c44b2" />



## 5. Lessons Learned 

The biggest lesson I learned from this project was the importance of considering printing time before finalizing a design. My original sock holder would have taken over 15 hours to print, which made me realize that I needed to adjust the size. Instead of starting over, I scaled the design down to 40% and found another useful purpose for it. This taught me that a design can be modified to solve a different problem without having to create an entirely new model. I also learned how scaling affects the overall dimensions, wall thickness, material consumption, and printing time. Using PrusaSlicer helped me better understand how to prepare a model for printing and evaluate whether my design was practical. If I were to do this project again, I would consider the printing time and desired size earlier in the design process.

### Time and Resources

| Activity | Time |
|---|---|
| Researching and choosing a design | 1 hour |
| Designing in SolidWorks | 25 minutes |
| Estimated printing time | 1 hour 33 minutes |
| Total estimated time | 2 hours 58 minutes |

The resources I used were SolidWorks, PrusaSlicer, PETG filament, and the PC-10 3D printer. The total above uses the slicer's estimated print time rather than a confirmed actual print duration.

## 6. Conclusion

Overall, this project allowed me to create a functional desk organizer using SolidWorks and 3D printing. Although my original idea was a sock holder, reducing the model's size made it more practical for everyday use. The final design provides a place to store my keys, AirPods, cologne, and other smaller belongings. This project helped me improve my SolidWorks modeling skills and taught me to consider size, printing time, and functionality when designing a product.

## 7. Reference

[Great Questions Lead to Great Design: A Guide to the Design-thinking Process – Toptal](https://www.toptal.com/designers/product-design/design-thinking-great-questions)

