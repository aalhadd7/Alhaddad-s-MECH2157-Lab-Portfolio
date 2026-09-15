# Lab 4 – Pull Strength Test

## Parameter and Prediction

For this project, I chose to benchmark the **pull strength** of a PLA part printed on the Prusa CORE One.

I designed a tensile-test specimen in SolidWorks with a narrow center section so that the highest stress would be concentrated near the middle of the specimen during the pull test.

The specimen dimensions were:

- Overall length: **165 mm**
- End width: **19 mm**
- Center width: **6.5 mm**
- Thickness: **3 mm**

Before testing, I predicted that the specimen would fail in the narrow center section because it had the smallest cross-sectional area.

My predicted maximum load was approximately **500 N or about 112 lbf** based on the specimen's PLA material, **6.5 mm × 3 mm center section**, **15% infill**, and **2-perimeter print settings** as a reasonable expected failure load before testing.

<img width="1613" height="846" alt="image-5" src="https://github.com/user-attachments/assets/144a1a05-5e03-4543-8f65-f20a6bbd7432" />


<img width="1793" height="735" alt="image-4" src="https://github.com/user-attachments/assets/e58553b1-854f-4054-8149-44537643552c" />


---

## Design Process

I created the tensile specimen in SolidWorks using a symmetric design with wider gripping sections and a reduced center section.

The wider ends allowed the specimen to be held during the pull test, while the narrow center section was designed to create the highest stress and provide a controlled failure location.

The design used gradual transitions between the wide ends and the narrow center instead of a sudden change in width.

The completed dimensions included:

- Overall length: **165 mm**
- End width: **19 mm**
- Center width: **6.5 mm**
- Thickness: **3 mm**
- Right gripping section length: **38 mm**
- Transition dimension: **28.5 mm**
- Transition radius: **76 mm**

After completing the sketch, I extruded the profile to a thickness of 3 mm and exported the finished model as an STL file.


---

## Preprocessor

The STL file was imported into **PrusaSlicer** and prepared for printing on the Prusa CORE One using PLA.

### Print Settings

- Printer: **Prusa CORE One**
- Nozzle: **0.4 mm**
- Material: **Generic PLA**
- Layer height: **0.20 mm**
- First layer height: **0.20 mm**
- Infill: **15%**
- Infill pattern: **Grid**
- Perimeters: **2**
- Top solid layers: **5**
- Bottom solid layers: **3**
- Scale: **100%**
- Supports: **None required**

### Infill

I used **15% grid infill**. This provided internal structure while still allowing the specimen to represent a normally printed FDM part rather than a completely solid piece.

### Build Orientation

The specimen was printed **flat on the build plate**.

This orientation provided a large contact area with the print bed, kept the specimen stable during printing, and eliminated the need for supports.

### Supports

No supports were required because the specimen was positioned flat and did not contain major unsupported features.

### Scale

The model was kept at **100% scale** so that the original dimensions and cross-sectional area would remain unchanged.

Changing the scale would have changed the dimensions of the center test section and affected the pull-strength results.

### Temperature and Settings

The PLA printing temperatures were:

- First-layer nozzle temperature: **230°C**
- Other-layer nozzle temperature: **220°C**
- Bed temperature: **60°C**


<img width="1109" height="895" alt="image-2" src="https://github.com/user-attachments/assets/56b3c475-08ff-4400-b14c-7b3b7d062c00" />



<img width="792" height="303" alt="image-1" src="https://github.com/user-attachments/assets/fda741fc-816a-46d5-b78c-9baf9f962554" />


<img width="1029" height="459" alt="image" src="https://github.com/user-attachments/assets/7d244242-4fb2-478a-9c27-db89156ed272" />



---

## Slice Information

After slicing the specimen, PrusaSlicer estimated:

- Estimated print time: **10 minutes**
- Stealth-mode estimate: **12 minutes**
- Used filament: **5.73 g**
- Filament length: **1.92 m**
- Filament volume: **4617.58 mm³**
- Estimated material cost: **$0.15**

<img width="2048" height="1048" alt="image-3" src="https://github.com/user-attachments/assets/60a7d336-79ed-4be8-9692-0335f231bcfb" />


---

## Print Artifact

The artifact was printed to test the **pull strength of a PLA FDM print**. The wider ends of the specimen were used as gripping areas, while the narrow center section acted as the main testing area. 
The design was successfully printed and then physically tested until failure.

<img width="407" height="334" alt="Screenshot 2026-09-15 at 12 08 13 PM" src="https://github.com/user-attachments/assets/28e50e08-aff1-4bf5-842d-1aacfdacdde3" />



https://github.com/user-attachments/assets/4bd4ad07-73b5-4b39-bea3-d6e388106a6a





---

## Pull Strength Test

To perform the test, I used a **pair of pliers to securely grip one side of the specimen**.

On the opposite side, I wrapped a **luggage scale around the specimen** so that I could measure the pulling force.

I gradually increased the pulling force until the specimen failed.

The luggage scale recorded a maximum load of: **117 lbf**

This is approximately: **520 N**

The test gave me a measurable value for the actual force required to break the printed PLA specimen.


<img width="524" height="280" alt="Screenshot 2026-09-15 at 12 09 36 PM" src="https://github.com/user-attachments/assets/ac5aa235-bd5f-418c-9f7f-78b56d5dba3c" />


---

## Test Results

### Maximum Load Before Failure

**117 lbf** or approximately **520 N**

My original prediction was approximately **112 lbf**, so the actual result was very close to my prediction.

The difference between the prediction and actual result was only about **5 lbf** off. The actual specimen was therefore slightly stronger than I originally predicted.

### Approximate Tensile Stress

The narrow section of the specimen had a cross-sectional area of:

**6.5 mm × 3 mm = 19.5 mm²**

Using the measured force: **520 N**

The approximate tensile stress at failure was: **26.7 MPa**

This provides another way to describe the strength of the specimen based on both the force and the dimensions of the center section.

---

## Lessons Learned

### 1. Cross-Sectional Area

The narrow center section played an important role in the pull test because it had less material available to resist the applied load than the wider gripping sections.

This showed how changing the cross-sectional area can directly affect where stress is concentrated in a part.

### 2. Prediction Compared to Actual Result

I predicted that the specimen would fail at approximately **112 lbf**.

The actual maximum load was **117 lbf**, meaning my prediction was very close to the measured result.

The specimen was approximately **5 lbf stronger** than predicted.

### 3. Build Orientation

Printing the specimen flat allowed it to be printed without supports and maintained the same orientation throughout the entire artifact.

The orientation of an FDM print is important because the direction of the printed layers can influence how the part reacts to an applied load.

### 4. Testing Method

Using a **luggage scale** allowed me to measure the force instead of simply pulling the specimen apart by hand and estimating the strength.

The pliers helped me securely grip one side while the luggage scale was used to apply and measure the pulling force on the other side.

This gave me a measurable maximum load of **117 lbf**.

---

## Conclusion

The pull-strength test successfully measured the strength of my PLA specimen.

My predicted failure load was approximately **112 lbf**, while the actual specimen reached **117 lbf** before failure.

This showed that the actual result was very close to my original prediction.

The experiment also demonstrated how **cross-sectional area, print orientation, infill, geometry, and FDM printing parameters** can affect the strength of a printed part.

If I repeated the experiment, I would test multiple identical specimens and average their results. This would provide a more reliable measurement and show how consistent the printing process is from one specimen to another.

---

## Resources

1. Prusa Research – Prusa CORE One
2. Prusament PLA Technical Information
3. Class Design Rules for 3D Printing
