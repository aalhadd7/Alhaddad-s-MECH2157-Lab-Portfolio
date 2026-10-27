# Laser Cutting Lab: Parametric Construction Kit

## Part 1: Group Work – Material Measurements and Fit Testing

### 1. Measuring the Laser Kerf

We began this project by measuring the kerf of the laser cutter to determine how much material was removed during cutting. This was important because the dimensions entered in SolidWorks do not always match the dimensions of the finished wooden pieces. Understanding the kerf would help us design joints that fit together properly.

To measure the kerf, we created a 20 mm × 20 mm square in SolidWorks. We then exported the design as a PDF and prepared it for cutting using Inkscape and the Epilog laser cutter. We placed our wooden sheet inside the machine, positioned the design, and performed the cut.

<img width="580" height="539" alt="Screenshot 2026-10-27 at 11 59 29 AM" src="https://github.com/user-attachments/assets/17fd72ff-d1b5-424b-9ccb-58a5824730a4" />


<img width="779" height="345" alt="Screenshot 2026-10-27 at 12 00 10 PM" src="https://github.com/user-attachments/assets/ac2d4091-552e-49c5-8eb4-4688215d386a" />



After cutting the square, we used digital calipers to measure its dimensions in both directions. Although the original design was 20 mm × 20 mm, the actual measurements were 19.61 mm and 19.48 mm.

We calculated the kerf using the following formula:

**Kerf = Designed Dimension − Actual Dimension**

- X-direction: 20.00 − 19.61 = **0.39 mm**
- Y-direction: 20.00 − 19.48 = **0.52 mm**

The measurements showed that the laser removed slightly different amounts of material in each direction. For our calculations, we decided to use a kerf value of **0.52 mm**, which represented the greater dimensional difference and helped us account for the variation.

<img width="523" height="519" alt="Screenshot 2026-10-27 at 12 00 50 PM" src="https://github.com/user-attachments/assets/7c357ce5-d4d7-4d1d-9b57-6394446915d9" />

<img width="528" height="513" alt="Screenshot 2026-10-27 at 12 01 06 PM" src="https://github.com/user-attachments/assets/99fc4f5b-a43b-4232-a50b-115b542082da" />



### 2. Measuring Material Thickness and Calculating Slot Width

The next step was to determine the actual thickness of our wooden sheet. Instead of relying only on the nominal thickness of 1/8 inch, we used digital calipers to measure the material. The thickness value used in our SolidWorks equations was **2.72 mm**.

Using this thickness and our measured kerf, we calculated a slot width that would allow the pieces to connect securely without being too difficult to assemble.

We used the following equation:

**Slot Width = Material Thickness − Kerf + Clearance**

We selected an initial clearance allowance of 0.30 mm.

**Slot Width = 2.72 − 0.52 + 0.30**

**Calculated Slot Width = 2.50 mm**

Based on this calculation, we predicted that a **2.50 mm slot opening** would produce a good fit. However, we wanted to test several dimensions around this value before finalizing the design.

### 3. Designing and Testing Different Slot Openings

To determine the best opening, we created a fit-test piece in SolidWorks. The test piece was a 40 mm × 40 mm square containing five slots, each with a length of 20 mm. We varied the slot widths to compare how tightly the wooden pieces would fit.

The five openings were:

| Test | Designed Slot Width |
|---|---|
| 1 | 2.40 mm |
| 2 | 2.50 mm |
| 3 | 2.60 mm |
| 4 | 2.70 mm |
| 5 | 2.80 mm |

<img width="738" height="556" alt="Screenshot 2026-10-27 at 12 01 29 PM" src="https://github.com/user-attachments/assets/d3eaa0aa-7984-4a73-a9ab-e82fc2ae85ac" />


After completing the design, we exported it for laser cutting and prepared the file using the Epilog Dashboard. We selected the wood-cutting settings and arranged the test piece on the material.
<img width="610" height="460" alt="Screenshot 2026-10-27 at 12 02 14 PM" src="https://github.com/user-attachments/assets/96f686cc-f678-418b-ad4a-5b620a859e76" />


Once the fit-test piece was cut, we tested the openings by inserting a wooden piece into the different slots. This allowed us to physically compare the fit rather than relying only on calculated dimensions. The tighter openings required more force to insert, while the wider openings provided additional clearance. Our goal was to find a connection that could be assembled without damaging the wood while still holding the pieces securely. Our calculated target of 2.50 mm provided the starting point for these tests. Testing additional widths helped us understand how small dimensional changes can affect the final connection.

<img width="343" height="306" alt="Screenshot 2026-10-27 at 12 02 52 PM" src="https://github.com/user-attachments/assets/af3fa6af-1a00-43c3-b71c-d943b3e9ec50" />


### 4. Group Results and Final Decision

Through our group testing, we learned that kerf and material thickness both have a significant effect on the accuracy of laser-cut joints. Our measurements showed that even a small difference between designed and actual dimensions can change how tightly two pieces connect. We used 2.50 mm as our target slot width based on the measured material thickness, kerf, and selected clearance. Testing additional slot widths gave us a practical way to evaluate the fit before applying the dimensions to our individual designs. This process demonstrated the importance of testing multiple parameters instead of assuming that a single calculated value will always produce the best result.

---

## Part 2: Individual Work – Parametric Construction Kit

## Design

### 1. Creating My Construction Kit in SolidWorks

After completing the group measurements and testing, I began designing my own parametric construction kit in SolidWorks. The objective was to create at least three unique part types and eight total pieces that could connect using laser-cut slots. I decided to create three different shapes: a circle, a square, and a rounded rectangle. I chose these shapes because they were simple to design, easy to manufacture, and provided different geometries that could be connected to form a three-dimensional structure.

My original designs included:

- **Circle:** 30 mm diameter.
- **Square:** 20 mm × 20 mm.
- **Rounded rectangle:** 20 mm straight middle section with 8 mm end radii.

Each shape included a centered slot designed to allow it to connect with another wooden piece. The slot dimensions were based on the kerf and clearance calculations completed during our group testing.

<img width="536" height="278" alt="Screenshot 2026-10-27 at 12 03 42 PM" src="https://github.com/user-attachments/assets/313e5661-c16e-4b39-ad23-42d528a47460" />



After drawing the shapes, I used the Extruded Boss/Base feature to turn the sketches into three-dimensional models. This allowed me to visualize how the pieces would look after being cut from the wooden sheet.

<img width="682" height="249" alt="Screenshot 2026-10-27 at 12 04 38 PM" src="https://github.com/user-attachments/assets/e3186b19-9bc3-430e-abf6-a302b3c584be" />


### 2. Using Global Variables and Equations

An important requirement of this project was making the design parametric. Rather than relying only on manually entered dimensions, I created global variables in SolidWorks to control the dimensions of my pieces and their connection slots.

I went to **Tools → Equations** and entered the following variables:

| Variable | Value | Purpose |
|---|---|---|
| `k` | 0.52 mm | Measured kerf |
| `t` | 2.72 mm | Material thickness |
| `w` | 20.00 mm | Piece width |
| `c` | 0.30 mm | Clearance |
| `s` | 2.50 mm | Calculated slot opening |

For the slot opening, I entered the equation:

**s = t − k + c**

**s = 2.72 − 0.52 + 0.30 = 2.50 mm**

The purpose of these equations was to make it easier to modify the design when material thickness or cutting conditions changed. By linking the slot dimensions to the global variables, the model can automatically update when one of the controlling values is adjusted.

For example, increasing the material thickness variable from 2.72 mm to 2.82 mm would change the calculated slot opening from 2.50 mm to 2.60 mm, assuming the kerf and clearance remained constant.

This approach is more efficient than manually changing each slot and helps maintain consistency between all the pieces.

<img width="1341" height="633" alt="Screenshot 2026-10-27 at 12 05 06 PM" src="https://github.com/user-attachments/assets/4ecdfc97-077b-45ae-bf3b-3c35ce14634c" />


### 3. Finalizing the Design

Once the individual shapes and their connection slots were designed, I reviewed the dimensions to make sure the pieces could connect properly. I used the results from our group fit testing to guide the slot dimensions.

I then prepared the parts for laser cutting. My final layout contained three copies of each unique shape, giving me a total of nine individual pieces.

This satisfied the requirement for at least three unique part types and eight total pieces. Using several copies of each shape also allowed me to experiment with different arrangements during assembly.

## Manufacturing, Including Process Research

### 1. Researching Laser Cutting as a Manufacturing Process

Laser cutting is a manufacturing process that uses a focused, high-powered laser beam to cut through material. The laser follows a digital design and removes material through heating and vaporization or combustion. This process is commonly used for wood, acrylic, plastics approved for laser cutting, and certain metals. One advantage of laser cutting is its ability to produce detailed two-dimensional shapes quickly and consistently. Compared with FDM 3D printing, laser cutting is generally faster for producing flat components because it does not need to build the entire part layer by layer. Laser cutting can also create clean, repeatable outlines with relatively little material waste when the parts are arranged efficiently. However, laser cutting is generally limited to cutting flat sheets, while FDM printing can produce three-dimensional objects with more complex geometries. FDM printing also allows internal features and shapes that would be difficult or impossible to manufacture using only a laser cutter. For this project, laser cutting was the better manufacturing method because the construction kit consisted of flat wooden pieces that could be assembled into a three-dimensional structure. It allowed me to manufacture multiple parts from one sheet without needing to print each part individually.

### 2. Preparing the Design in Inkscape

After finishing my SolidWorks model, I exported the cutting geometry and transferred it into Inkscape to prepare the laser-cutting layout. I arranged the shapes in three rows, with one circle, one square, and one rounded rectangle in each row. This arrangement made the pieces easy to identify and provided spacing between the different parts. I also checked that the outlines and internal slots were correctly positioned before sending the design to the laser cutter.

**[Insert Picture 13: Final Inkscape layout showing all nine pieces]**

### 3. Laser Cutter Setup and Settings

For manufacturing, I used the Epilog laser cutter and selected the cutting preset for 1/8-inch (3 mm) wood.

The laser settings recorded in the Epilog Dashboard were:

| Setting | Value |
|---|---|
| Machine | Epilog CO₂ Laser Cutter (SFL LA-4) |
| Material | Wood |
| Nominal thickness | 1/8 inch (3 mm) |
| Measured thickness used in CAD | 2.72 mm |
| Process type | Vector |
| Speed | 15% |
| Power | 100% |
| Frequency | 20% |
| Number of passes | 1 |
| Autofocus | Off |
| Vector sorting | Inside-Out |
| Estimated cutting time | 59 seconds |

I imported my design into the Epilog Dashboard and selected the appropriate wood-cutting settings. I checked the positioning of the shapes and confirmed that they were located within the available material. Using the same cutting settings helped maintain consistency between the different parts. I also checked the alignment before cutting to reduce the chance of cutting outside the intended material area.

<img width="1105" height="471" alt="Screenshot 2026-10-27 at 12 06 23 PM" src="https://github.com/user-attachments/assets/2a9f0307-f17c-4277-bd55-66d2a6dba7a4" />


### 4. Cutting and Inspecting the Wooden Pieces

After preparing the laser cutter, I proceeded with cutting my design. The machine followed the outlines and internal slots of each shape to produce the nine wooden pieces. Once the cutting process was complete, I removed the pieces and inspected the edges and slots. The laser produced darkened edges because of the heat used during cutting. This is a common characteristic of laser-cut wood. The air-assist and exhaust systems are important during laser cutting because they help remove smoke and debris from the cutting area. Proper airflow can also help reduce excessive burning and improve the appearance of the finished edges. I inspected the pieces to make sure the slots were fully cut and that the components could be assembled without major interference.

### 5. Assembling My Construction Kit

After cutting the wooden pieces, I began assembling my construction kit. I used the slots to connect the circles, squares, and rounded rectangles in different orientations. Rather than building one fixed structure, I experimented with different connections to demonstrate how the same pieces could be rearranged into multiple configurations. The final assembly demonstrated how flat laser-cut components could be combined into a three-dimensional structure without requiring screws or other permanent fasteners. This was also an opportunity to evaluate the slot dimensions from our earlier testing. The connections needed to provide enough grip to hold the pieces together while still allowing them to be assembled by hand.


<img width="266" height="277" alt="Screenshot 2026-10-27 at 12 06 58 PM" src="https://github.com/user-attachments/assets/5535572c-5a99-4812-88c4-b932a1dad57d" />


## Lessons Learned

### 1. Importance of Accurate Measurements

One of the most important lessons from this project was understanding how small measurement errors can affect the final product. Our original kerf test was designed as a 20 mm square, but the actual dimensions were 19.61 mm and 19.48 mm. If we had assumed that the laser would cut the exact dimensions entered in SolidWorks, our slots might have been too loose or too tight. By measuring the kerf and accounting for the actual material thickness, we were able to make a more informed decision when designing the connections. This project reinforced the importance of measuring real materials and testing manufacturing results rather than relying entirely on theoretical dimensions.

### 2. Testing Different Clearances

Another important lesson was that even a small change in slot width can affect how wooden components fit together. Although we calculated an ideal opening of 2.50 mm, we tested five different widths ranging from 2.40 mm to 2.80 mm. This allowed us to evaluate how clearance affected assembly and connection strength. This testing relates to Genichi Taguchi's concept of robust design, which emphasizes producing parts that continue to function properly even when small manufacturing variations occur. For example, a joint might technically connect but still have too much movement. According to Taguchi's quality loss concept, a connection that moves away from its intended fit can create quality losses even if the parts can still be assembled. If thousands of these parts were manufactured, small fit errors could lead to inconsistent assemblies, greater wear, or increased rejection rates.

### 3. Troubleshooting and Design Improvements

One challenge during the project was accounting for the difference between the dimensions in SolidWorks and the actual size of the laser-cut pieces. The original square dimensions did not match the finished part, which showed why kerf compensation was necessary. We addressed this issue by measuring the cut square and testing several slot dimensions. Rather than immediately producing our final construction kits, we used the fit test to evaluate which openings would work. Another consideration was ensuring that the internal slots were accurately positioned and that the pieces could connect without damaging the wooden material. If I had another opportunity to improve the design, I would perform additional fit tests using smaller changes around the selected 2.50 mm opening. This would help me determine a more precise clearance and improve consistency between the connections.

### 4. Real-World Applications

A real-world application of this type of manufacturing is flat-pack furniture, where wooden or sheet components are cut and joined together during assembly. If the slots or tabs were manufactured with incorrect dimensions, customers might have difficulty assembling the furniture. A slot that was too small could require excessive force and potentially damage the material, while a slot that was too large could result in an unstable connection. This is why accurately accounting for manufacturing tolerances is important when designing products intended for repeated production.

### 5. Resources Used

The resources and equipment used for this project included:

- SolidWorks for parametric CAD modeling and global variables.
- Inkscape for preparing the laser-cutting layout.
- Epilog CO₂ laser cutter and Epilog Dashboard.
- 1/8-inch nominal wooden sheet material.
- Digital calipers for measuring kerf and material dimensions.
- Computer for creating and exporting the cutting files.
- Wooden kerf and fit-test coupons.
- Wooden construction kit components.

### 6. Process Log

The following process log documents the major stages of the project.

| Step | What Happened | Decision or Change Made |
|---|---|---|
| 1 | Designed a 20 mm square in SolidWorks. | Used the square to measure kerf. |
| 2 | Cut the square and measured it using digital calipers. | Selected 0.52 mm as the kerf value for calculations. |
| 3 | Measured the material thickness. | Used 2.72 mm in the parametric equations. |
| 4 | Calculated the target slot opening. | Selected 2.50 mm as the initial target. |
| 5 | Designed a fit-test piece with five different slot widths. | Tested widths from 2.40 mm to 2.80 mm. |
| 6 | Created three unique construction kit shapes in SolidWorks. | Used circles, squares, and rounded rectangles. |
| 7 | Created global variables and equations. | Made the slot calculation dependent on thickness, kerf, and clearance. |
| 8 | Prepared nine pieces in Inkscape. | Arranged three copies of each shape. |
| 9 | Prepared and performed the laser cut. | Used the 1/8-inch wood vector-cutting settings. |
| 10 | Inspected and assembled the pieces. | Tested different three-dimensional configurations. |

**Total Project Time:** 8 hours

### 7. Final Reflection

Overall, this project helped me better understand the relationship between CAD design, manufacturing accuracy, and physical assembly. It demonstrated that creating a design in SolidWorks is only part of the manufacturing process. The actual material properties and the precision of the machine must also be considered. By measuring kerf, testing multiple clearances, and creating global variables, I learned how to design parts that better account for manufacturing variations. The final construction kit demonstrated how simple two-dimensional shapes could be manufactured and assembled into a three-dimensional structure. The biggest takeaway from this project was the importance of testing and adjusting a design using actual measurements instead of assumptions.

## Final Laser Cutting Video

Below is a 15-second clip showing the laser cutter manufacturing the wooden components for my construction kit.

<img width="180" height="320" alt="IMG_2604" src="https://github.com/user-attachments/assets/70f74ecb-d906-479d-a28d-79267c7eaa2c" />

