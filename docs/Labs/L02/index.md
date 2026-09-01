# Lab 2 - Design and Slicing

## Individual Research DfAM


A common Design for Additive Manufacturing guideline is the 45 degree rule. For many 3D-printing processes, surfaces angled about 45° or more from the build plate can support themselves, while shallower overhangs may require extra support material. This matters because reducing supports can save material, shorten printing time, and reduce the work needed after printing.

## Individual Research: FDM

Warping is an issue in FDM printing where the plastic shrinks as it cools, which can cause the corners of a part to lift off the print bed. A designer can reduce warping by avoiding sharp corners when possible, improving the part’s contact with the build plate, or using features such as a brim to help hold the part down during printing.

## What I learned 

Two things that I learned was how changing the orientation of a part can reduce the amount of support material needed during printing. Also, I learned that using a heated print bed can help prevent warping by keeping the bottom of the part warm.


# Lab 2 – FDM 3D Printing

## Download

For this lab, I used Printables.com to search for a small model that would meet the requirements of the assignment. I looked for models that were simple, had a flat surface for printing, could be scaled down easily, and would have a short print time.

### My First Choice

While searching, I considered multiple different models before making my final selection. Some of the other models were more complicated, would require more support material, or would take longer to print.

<img width="547" height="415" alt="Screenshot 2026-09-01 at 11 34 25 AM" src="https://github.com/user-attachments/assets/980292cc-75e1-4a48-914b-dfdd5cfa1cd1" />

<img width="579" height="361" alt="Screenshot 2026-09-01 at 11 35 09 AM" src="https://github.com/user-attachments/assets/6e251ede-a456-4fae-996b-05aea4bc559a" />


This is the first design I wanted to print out. I alway loved fidget spinners as a kid and thought it would be cool to make that my first 3D print. But it seemed a bit too complex for this task having almost an hour print time. So I decided to do something smaller and simpler. 

I decided to use a cable holder because it had a simple design, had a suitable surface to print from, and could easily be scaled down to meet the size requirements of the assignment. Its small size also helped keep the printing time short and it doesn't need any support.

### Cable Holder 

The Cable Holder was downloaded from Printables as an STL file using the following link:

https://www.printables.com/model/206748-cable-holder/files


<img width="964" height="720" alt="Screenshot 2026-09-01 at 12 14 09 PM" src="https://github.com/user-attachments/assets/19885d9b-4902-40a8-a6de-d6f2d188503b" />

I chose the cable holder because it had a relatively simple design and could easily be scaled down to meet the size requirements of the assignment. It also had a suitable surface to build from and could be printed quickly.

After choosing the model, I downloaded the STL file from Printables. The STL file contained the geometry of the model and was later imported into PrusaSlicer to prepare it for printing.

After downloading the STL file, I imported it into PrusaSlicer so that it could be scaled, oriented, and converted into G-code for the 3D printer.

For this lab, I used Printables to search for a small 3D model that could be manufactured using an FDM printer. The model needed to meet the assignment requirements of being no more than 0.25 inches tall, no larger than 2 inches by 2 inches, printed using PLA, and completed in less than 1.5 hours, realistically under 30 minutes .

While searching, I considered multiple designs before choosing my final model. I looked for something that had a simple shape, could be scaled down easily, had a stable surface to print from, and would not require a long printing time.

## Preprocessor

### Importing the STL File

After downloading the STL file, my group imported our models into PrusaSlicer. Mohammad helped the group by collecting the STL files that each of us downloaded so that all four parts could be prepared for printing.

<img width="660" height="417" alt="Screenshot 2026-09-01 at 11 45 30 AM" src="https://github.com/user-attachments/assets/84d79201-4b92-4968-a25c-738db0fb3b41" />

### Scaling

The cable holder was scaled down in PrusaSlicer. The main reason for scaling the model was to make sure it met the required dimensions while also keeping the printing time relatively short.

Since this part was being used to demonstrate the FDM printing process, it did not need to remain at its original size. Scaling it down also reduced the amount of PLA needed.


### Build Orientation

I oriented the cable holder so that its flat surface was placed against the build plate. This provided a stable base for the model and helped with adhesion during the beginning of the print.

The orientation also helped reduce the need for unnecessary support material.

### Supports

The model did not require a large amount of support material because of its size, shape, and orientation.

In PrusaSlicer, the support setting was set to **"For support enforcers only."**

This allowed the model to be printed without adding unnecessary supports that could increase material usage and printing time.

### Infill

The model was prepared using **15% infill**. Since the cable holder was small and this print was mainly being used to demonstrate the FDM manufacturing process, a high infill percentage was not necessary.

Using 15% infill also helped reduce the amount of filament and printing time.

### Material

The material used for the assignment was **PLA**. Prusament PLA was selected when preparing the model in PrusaSlicer.

### Print Settings

The model was prepared using approximately **0.20 mm layer settings**.

After the settings were selected, PrusaSlicer converted the STL model into G-code. The G-code contains the instructions that tell the 3D printer how to manufacture the model layer by layer.

<img width="342" height="404" alt="Screenshot 2026-09-01 at 11 58 06 AM" src="https://github.com/user-attachments/assets/48d1ab96-2f66-49f8-a068-dedf5c0eef99" />


### Slicing and Print Time

After slicing the model, I reviewed the PrusaSlicer preview to make sure the model would print correctly.

An earlier PrusaSlicer setup showed an estimated printing time of approximately 21 minuets. After the models were scaled and the final group print was prepared, all **four parts were placed into the same print job**. The final print took approximately 13 minuets total for all four parts, which was well below the assignment limit of 1.5 hours. The slicing process also allowed me to see how the printer would create the different sections of the model, including the perimeters, infill, solid infill, and bridges.


## Print

### Preparing the Print

Because the UNCC print farm had a limited number of working printers, my partners and I printed our models together.

Four different parts were placed into the same print job so that we could use one printer instead of using separate printers for each person.

<img width="435" height="347" alt="Screenshot 2026-09-01 at 11 41 22 AM" src="https://github.com/user-attachments/assets/54d742ef-b71c-42ce-b907-d89e74855a98" />


The printer screen displayed all four models arranged on the build platform before the print began.

The final group print required approximately **5 grams of PLA** and had a printing time of approximately **13 minutes**.


### First Printer Error

One problem that occurred during the lab happened when we attempted to use our first printer.

The first printer experienced an error and we were unable to continue the printing process using that machine. Because of this, we had to switch to another printer and load our print onto the new machine.

This showed me that even if the STL files and G-code are prepared correctly, problems with the actual printer can still affect the manufacturing process.

<img width="682" height="277" alt="Screenshot 2026-09-01 at 11 42 10 AM" src="https://github.com/user-attachments/assets/38c2c5e1-b7ff-4399-823c-b64b01776de4" />

### Second Printing Attempt

After switching to another printer, we loaded the G-code onto the new machine and started the printing process again.

Before the actual printing began, the printer had to heat the nozzle and build plate to the temperatures required for PLA.

Once the correct temperatures were reached, the printer began creating the four parts one layer at a time.

### Printing Process

During the print, we monitored the printer to make sure that the parts were properly adhering to the build plate and that there were no additional errors.


The printing process took approximately 25 minutes with the first printer error. 

A short video of approximately 15 seconds was also taken during the printing process to document the printer operating.

**Video:** 

https://github.com/user-attachments/assets/edadae72-0308-43d2-a1e7-dc9cccef4506





### Completed Print

The second printer successfully completed the print. This is a front and back picture of the completed print. 

<img width="378" height="262" alt="Screenshot 2026-09-01 at 12 08 16 PM" src="https://github.com/user-attachments/assets/7c3af359-7ddd-4457-a078-24fa58353859" />

<img width="247" height="210" alt="Screenshot 2026-09-01 at 12 08 38 PM" src="https://github.com/user-attachments/assets/21579921-fa4c-489a-9ee9-27c86a3bd49c" />



The final cable holder met the size and printing-time requirements for the assignment. The finished physical part was also brought to lab as required.


## Partners and Acknowledgements

I completed this lab with Mohammad and my other lab partners.

Mohammad was especially helpful during the preprocessing portion of the lab because he collected the STL files that each member of the group downloaded and helped combine them so that all four models could be printed together.

My partners also helped throughout the printer setup and troubleshooting process, especially when the first printer experienced an error and we had to switch to another printer.

---

## Lessons Learned

### 1. Model Size Affects Print Time

One thing I learned during this lab was how much the size of a model affects its printing time. Scaling the cable holder down reduced both the amount of material required and the amount of time required to print it.

### 2. Build Orientation Is Important

I learned that the orientation of a model on the build plate can affect how successfully it prints. Placing a flat surface against the build plate provides better stability and can reduce the amount of support material needed.

### 3. PrusaSlicer Converts an STL File Into Printer Instructions

I learned the purpose of slicing software in the 3D printing process. The STL file contains the geometry of the model, while PrusaSlicer converts that model into G-code that the printer can follow to manufacture the object layer by layer.

### 4. Printer Problems Can Occur

I learned that preparing the model correctly does not guarantee that the print will immediately work. Our first printer experienced an error, which required us to switch to another printer.

This showed me that troubleshooting the physical equipment is also an important part of the 3D printing process.

### 5. Multiple Parts Can Be Printed Together

I learned that multiple small models can be arranged on the same build plate and manufactured during the same print.

Our group printed **four different parts together in approximately 13 minutes**. This allowed us to use the limited number of printers in the lab more efficiently.

---

## What I Would Change

If I completed this lab again, I would check that the printer was fully operational before beginning the print. This could prevent time from being lost because of a printer error.

I would also spend more time comparing different scales and orientations in PrusaSlicer before generating the final G-code. Small changes to the size and orientation of the model can affect printing time, material usage, supports, and the overall quality of the finished part.

---

## Total Time

The Entire project took us about 45 minutes. From downloading the file to completing the print. Time was required for searching for a model, downloading the STL file, preparing the models in PrusaSlicer, and troubleshooting the first printer.

---

## Resources

- **Printables** – Used to locate and download the Cable Holder STL file.
- **Cable Holder Model:** https://www.printables.com/model/206748-cable-holder/files
- **PrusaSlicer** – Used to scale, orient, slice, and convert the STL files into G-code.
- **UNCC Rapid Lab** – FDM printer and PLA material used to manufacture the final parts.
- Professor Fagan
