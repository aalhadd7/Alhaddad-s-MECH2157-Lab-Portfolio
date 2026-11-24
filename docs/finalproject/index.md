# MEGR 2156/7 L3D – Final Project: Shower Loofah Holder
## Part 1: Define the Problem and Rough Prototype 

###  Project Overview

For my final project, I designed a removable shower loofah holder that attaches to an existing shower rod. The problem I wanted to solve was not having a convenient place to hang my loofah, which would often fall or take up space in the shower. My goal was to create a holder that could snap onto the rod without drilling holes or making permanent modifications. One of the main challenges was that the shower rod slopes slightly downward, meaning a regular hook would not be positioned correctly. To address this, I designed an angled support that connects the rod attachment to a separate hook. The prototype uses two manufacturing technologies: Fused Deposition Modeling (FDM) for the snap-fit and supporting components, and Stereolithography (SLA) for the hook.

### 1. Research

#### 1.1 Spiral Design Process

The Spiral Design Process consists of planning, risk analysis, engineering, and evaluation. Planning involves identifying the problem and determining the requirements. Risk analysis focuses on potential design issues, while engineering involves modeling and manufacturing the prototype. Evaluation involves testing the design and making improvements. I applied this process by measuring the shower rod, designing the components in SolidWorks, manufacturing the parts, and testing their fit. The problems identified during testing will guide my next design modifications.

#### 1.2 FDM Anisotropy

FDM printing creates parts by depositing melted material in layers, making the strength of the printed part dependent on its orientation. Parts are generally weaker between layers than within the layers themselves. This is important for my snap-fit attachment because it needs to flex when connecting to the shower rod. I considered the print orientation and wall thickness to reduce the possibility of the snap-fit breaking during installation.

#### 1.3 SLA Shrinkage

SLA printing uses resin that is cured using light. The material can experience shrinkage during printing and post-curing, which may affect dimensional accuracy. Since my hook was manufactured using SLA, I needed to consider how dimensional changes could affect its fit within the FDM-printed support. The final assembly showed that the connection had some looseness, indicating that the fitting dimensions still need adjustment. However, I have not confirmed whether SLA shrinkage contributed to this issue.

#### 1.4 Laser Cutting Kerf

Laser cutting removes a small amount of material along the cutting path, known as kerf. This must be considered when designing parts that require accurate dimensions or tight connections. One way to compensate for kerf is to create test cuts, measure the resulting dimensions, and adjust the original design. Although I did not use laser cutting for my prototype, understanding kerf is important when designing manufactured parts that must fit together.

### 2. Problem Definition

#### Problem 1: No Place to Hang My Loofah

My shower does not have a designated place for my loofah, causing it to fall or take up space. I wanted to create a holder that would keep it hanging securely and make it easier to access.

#### Problem 2: Angled Shower Rod

The shower rod is slightly angled downward, making it difficult to attach a hook that hangs in the correct position. This required an additional support component to compensate for the rod's angle.

#### Problem 3: Removable Attachment

I wanted a design that would attach directly to the rod without drilling or using permanent adhesives. The attachment needed to be removable while remaining secure enough to support the loofah.

### 3. Problem Selection

I selected the shower loofah holder because it addresses a problem I personally experience. I decided to use a snap-fit attachment that connects directly to the rod, an angled support to compensate for the slope, and a separate hook to hold the loofah. This project allowed me to use SolidWorks, dimensional measurements, FDM printing, SLA printing, and prototype testing to develop a functional solution.

### 4. Concept Development

#### 4.1 Measurements and Initial Design

Before modeling the components, I measured the shower rod to determine the approximate dimensions required for the attachment. These measurements provided a starting point for designing the snap-fit connection.

<img width="434" height="328" alt="Unknown-11" src="https://github.com/user-attachments/assets/15d33e68-0def-4dec-8c00-fa5faf1b1766" />

<img width="434" height="328" alt="Unknown-12" src="https://github.com/user-attachments/assets/6891094f-67d4-4e2b-a5db-db1e141327f2" />


#### 4.2 SolidWorks Design Development

I started by designing the snap-fit attachment that would connect directly to the shower rod. I created an angled profile in SolidWorks and used the Thin Extrude feature to give it thickness. The purpose of this component was to allow the holder to attach to the rod without using screws or adhesives.

<img width="875" height="490" alt="Unknown-3" src="https://github.com/user-attachments/assets/a8c0d05a-3647-4639-9a7f-ba0f4b356f35" />

<img width="825" height="602" alt="Unknown-4" src="https://github.com/user-attachments/assets/0b2fa039-6b14-4828-8d6e-c825a01ec61d" />

<img width="208" height="276" alt="Unknown-18" src="https://github.com/user-attachments/assets/dc388cfb-fe20-44da-8bed-aa55ec662d08" />


#### 4.3 Hook Design – SDP_HOOK

Next, I designed the hook that would hold the loofah. I created the profile in SolidWorks and used the Boss-Extrude feature to create the solid model. I designed the hook as a separate component so it could be inserted into the support instead of making the entire holder one piece.

<img width="2048" height="820" alt="Unknown" src="https://github.com/user-attachments/assets/08fc063d-ba60-4a66-9c7b-36eebc074c97" />

<img width="2048" height="913" alt="Unknown-1" src="https://github.com/user-attachments/assets/7c40aeed-3abb-44d7-9a92-f750987f0d70" />


<img width="2048" height="1045" alt="Unknown-2" src="https://github.com/user-attachments/assets/9207cef2-3793-42a3-8ae5-30b7b99ea020" />


#### 4.4 Design Modifications

The next challenge was correcting the downward angle of the shower rod. I designed an angled support with a triangular section that would allow the hook to sit closer to perpendicular to the floor. I also created a rectangular opening in the support where the hook could be inserted. After reviewing the original design, I modified the support dimensions to improve its geometry and the connection with the hook. I increased one dimension from 1.00 inches to 1.15 inches and another from 0.45 inches to 0.70 inches. I then used additional Cut-Extrude features to create the opening for the hook.

<img width="809" height="512" alt="Unknown-6" src="https://github.com/user-attachments/assets/b2674626-3b33-40de-961c-dff042b7ff65" />

<img width="2048" height="1024" alt="Unknown-7" src="https://github.com/user-attachments/assets/9ac45659-fc0f-409e-a6d2-f443364f8648" />

<img width="2048" height="1107" alt="Unknown-8" src="https://github.com/user-attachments/assets/19159220-22ec-4388-a2e5-965334deff25" />

<img width="2048" height="1040" alt="Unknown-9" src="https://github.com/user-attachments/assets/5c9c40c3-2af0-401a-92b2-6da10cc078b6" />


<img width="849" height="536" alt="Unknown-10" src="https://github.com/user-attachments/assets/97c5894d-eb70-4519-a5de-17d086eb1400" />


#### 4.5 FDM Printing

I used a Prusa CORE One printer with PETG filament to manufacture the snap-fit and angled support components.

The main printing settings included:

- Layer height: 0.20 mm
- Infill density: 15%
- Infill pattern: Grid
- Supports: None

I initially prepared the components in PrusaSlicer to examine their orientation and estimated material usage.

<img width="2048" height="1047" alt="Unknown-13" src="https://github.com/user-attachments/assets/145aa349-d1cc-458f-949e-b0c45eed5075" />

<img width="684" height="787" alt="Unknown-14" src="https://github.com/user-attachments/assets/404fc0c0-ceb8-4796-9f90-27ba6f894ba1" />

<img width="706" height="633" alt="Unknown-15" src="https://github.com/user-attachments/assets/4cb07acf-aab0-4afd-8073-82c8d081d332" />


I then printed the support component. The printer recorded a completed print time of 35 minutes and 55 seconds, using approximately 8 grams of PETG.

<img width="540" height="308" alt="Screenshot 2026-11-17 at 4 06 52 PM" src="https://github.com/user-attachments/assets/4cdc6fad-62f0-4e11-9972-217c0b3a01e5" />

<img width="262" height="209" alt="Unknown-17" src="https://github.com/user-attachments/assets/7a1584ff-2410-483e-9283-12e269bb680e" />

#### 4.6 SLA Printing

I used SLA printing to manufacture the separate hook component. SLA printing was useful for creating the detailed shape of the hook that would connect to the FDM support. This allowed me to combine two different manufacturing technologies in the final prototype.


<img width="100" height="177" alt="b64j06" src="https://github.com/user-attachments/assets/c8cc9ae5-894a-461d-9221-04a94c252782" />



<img width="301" height="276" alt="Unknown-16" src="https://github.com/user-attachments/assets/36e9d1a6-21e3-4782-a646-fb4dd894c7f7" />



### 5. Prototype Assembly and Testing

After manufacturing the components, I assembled the hook and support and attached the prototype to the shower rod. The holder was able to support the loofah, but testing revealed two problems that still need improvement.

#### 5.1 Snap-Fit Connection

The first issue was the snap-fit attachment. My initial fit was too tight on the shower rod. After modifying the design, the connection became too loose. This showed that the attachment dimensions need further adjustment to achieve a secure fit while still allowing the holder to be removed. I also thought it was too long for no reason so I decided to shorten it. 

<img width="309" height="218" alt="Screenshot 2026-11-17 at 4 39 17 PM" src="https://github.com/user-attachments/assets/3262173f-ac07-434d-b699-46d71c890bad" />



#### 5.2 Hook Connection and Alignment

The second issue was the connection between the hook and the angled support. Although the hook fits into the opening and can hold the loofah, the connection is not tight enough to maintain the intended perpendicular position consistently. To fix this, I would need to adjust the dimensions of the rectangular opening or the connecting section of the hook to reduce movement between the parts.

#### 5.3 Final Prototype Testing

Despite these issues, the assembled prototype demonstrated that the general design can hold the loofah on the shower rod. The remaining improvements involve making both connections more secure and maintaining the correct hook orientation.

<img width="328" height="268" alt="Unknown-19" src="https://github.com/user-attachments/assets/cd1ccb67-c691-4c81-9cbd-9944e52ac4e5" />


### 6. Project Video Presentation

I recorded a video explaining the problem and how my prototype was designed to solve it. The video explains why I needed the holder, how the angled shower rod influenced the design, and how the printed components connect to support the loofah.

https://github.com/user-attachments/assets/fd4ed841-db2d-40ce-a4b7-f1e961264ac5


### 7. Documentation 

In the early phases of projects I like to do a scrape brain dump on a piece of paper so that I can start visualizing what I want to design and what I would need to design it. I like to make little notes such as "get in." so that I can remember to measure my parts for example. It is definitely a my eyes only type of work as it is very informal and simply for mental clarification.

<img width="461" height="543" alt="Screenshot 2026-11-17 at 4 32 27 PM" src="https://github.com/user-attachments/assets/14dad12d-86bc-4648-a383-b7ff57ec2c67" />


### Reflection and Future Improvements

Throughout this project, I learned how important dimensional accuracy and tolerances are when designing components that fit together. Although the prototype was able to support the loofah, the connections were not as secure as I originally intended. The snap-fit attachment went from being too tight to too loose, showing that small dimensional changes can significantly affect the fit. I also learned that designing an angled support does not automatically guarantee the hook will remain perpendicular if the connection between the parts has too much clearance. For my next iteration, I would focus on adjusting the snap-fit dimensions and improving the connection between the SLA hook and FDM support. I would then test the revised prototype to determine whether the holder remains stable and maintains the correct alignment. Overall, this project gave me experience using two different 3D printing technologies and applying an iterative engineering design process to solve a real-world problem.


# MEGR 2156/7 L3D – Final Project: Shower Loofah Holder
## Part 2: Prototype Refinement & Final Presentation

### 1. Project Overview

For my final project, I designed a removable shower loofah holder that attaches directly to my shower rod. The purpose of this project was to create a convenient place to hang my loofah without drilling holes or permanently modifying the shower. The main design challenge was that my shower rod is angled downward. To solve this, I designed a snap-fit attachment with a triangular support that allows a separate hook to hang in a more perpendicular position. I used two manufacturing technologies for this project: FDM printing for the snap-fit and support, and SLA printing for the hook. For Part 2, I focused on refining my original design, improving the connections between the parts, and testing the prototype on the actual shower rod.

### 2. Peer Feedback and Reflection

During my Part 1 presentation, I received feedback from three classmates. Overall, they thought the problem was clearly defined and the design was practical. However, they also identified some areas that needed improvement.

#### Peer Feedback

**Candy Vasquez**

Candy mentioned that the design was easy to understand and could potentially hold other items besides a loofah. She also raised concerns about the tolerances between the FDM and SLA components.

**Austin Williams**

Austin thought the solution was practical but questioned whether the snap-fit would attach securely to the shower rod. He suggested making the connection tighter to prevent movement.

**Kaileigh Hill**

Kaileigh liked the triangular design and suggested making the fit tighter or potentially adding a counterweight to improve stability.

<img width="487" height="561" alt="Screenshot 2026-11-23 at 9 11 04 PM" src="https://github.com/user-attachments/assets/4d45eb3e-55ed-4b5c-9a84-d74c9bb2c25c" />


<img width="460" height="553" alt="Screenshot 2026-11-23 at 9 11 13 PM" src="https://github.com/user-attachments/assets/e84756a5-720d-419d-981c-4be36cfedb3f" />


<img width="450" height="194" alt="Screenshot 2026-11-23 at 9 11 20 PM" src="https://github.com/user-attachments/assets/a0bda49e-ce0b-45cc-9586-58e48eb6cf4a" />


<img width="472" height="590" alt="Screenshot 2026-11-23 at 9 11 36 PM" src="https://github.com/user-attachments/assets/9b367e84-4d0e-4104-bc86-140f3490493e" />


<img width="466" height="268" alt="Screenshot 2026-11-23 at 9 11 47 PM" src="https://github.com/user-attachments/assets/fe281be4-0385-4a7b-9b44-a5171259a129" />



#### Individual Reflection

After reviewing the feedback, I realized that the main issue was the fit between the components rather than the overall design. During my initial testing, the snap-fit went from being too tight to too loose after adjustments. The connection where the SLA hook attaches to the FDM support also had too much movement, preventing the hook from maintaining its intended position. Based on the feedback, I decided to focus on improving the geometry of the FDM component rather than redesigning the entire assembly.

### 3. Prototype Refinement

#### 3.1 SolidWorks Design Modifications

For Part 2, I returned to SolidWorks and modified my SDP_FD1 model.

I made three main changes:

1. Shortened one side of the snap-fit geometry to adjust how it connects to the shower rod.
2. Extended the section where the SLA hook inserts into the FDM support to improve the connection.
3. Changed the angle of the triangular cut to improve the positioning of the hook.

The updated design includes a triangular cut angle of 31.44° and a square opening dimensioned at 0.51 × 0.51 inches. These modifications were intended to address the concerns about the snap-fit connection, stability, and tolerances between the printed components.

<img width="609" height="488" alt="Unknown" src="https://github.com/user-attachments/assets/ce1e0641-3ec9-4352-b7d4-0d0f58fc70b8" />


<img width="761" height="423" alt="Unknown-1" src="https://github.com/user-attachments/assets/0cba243e-babc-4a2a-8504-e73c772b01bb" />


<img width="803" height="368" alt="Unknown-2" src="https://github.com/user-attachments/assets/7e6e50ce-deaf-4f91-ab20-f5ed7a6343a4" />


<img width="805" height="386" alt="Unknown-3" src="https://github.com/user-attachments/assets/ed07d5b1-dfa9-493f-9cdb-6f9949bc3037" />


<img width="684" height="422" alt="Unknown-4" src="https://github.com/user-attachments/assets/58daf48a-be0a-4b71-8611-169944906148" />


<img width="808" height="430" alt="Unknown-5" src="https://github.com/user-attachments/assets/b8498e30-3569-4dcc-9026-b7b479f82adf" />


#### 3.2 Parametric Design

I used dimensioned sketches in SolidWorks to control the geometry of the prototype. This allowed me to adjust the lengths of the support, the angle of the triangular cut, and the size of the opening where the hook attaches.

These dimensions made it easier to modify the model without starting the design from the beginning.

**INSERT SCREENSHOT HERE**

- Image 12 – SolidWorks equations or global-variable feature showing a dimension controlled by a parameter

### 4. Manufacturing the Refined Prototype

#### 4.1 FDM Printing

After completing the SolidWorks modifications, I exported the refined model into PrusaSlicer and prepared it for FDM printing.

I used the Prusa CORE One printer with the following settings:

- Material: PLA
- Layer height: 0.20 mm
- Infill density: 15%
- Infill pattern: Grid
- Perimeters: 2
- Supports: Enabled
- Support style: Snug

The estimated printing time was approximately 38 minutes, with 18.08 grams of filament.

<img width="884" height="442" alt="Unknown-6" src="https://github.com/user-attachments/assets/d083c63e-8252-4081-977c-75ee70bf5847" />


<img width="887" height="451" alt="Unknown-7" src="https://github.com/user-attachments/assets/26e50378-ead6-402a-9e38-b66164bdbb1e" />


<img width="500" height="537" alt="Unknown-8" src="https://github.com/user-attachments/assets/889959e5-0ce7-480d-9f6b-a27f8c953d52" />


<img width="569" height="460" alt="Unknown-9" src="https://github.com/user-attachments/assets/2d3d0e8c-aa85-4f4e-b5c9-4dd4824145d1" />


<img width="549" height="617" alt="Unknown-10" src="https://github.com/user-attachments/assets/8b217751-52c7-430b-b1ba-db4fe9e004ec" />



#### 4.2 FDM Printing Video

I also recorded a video showing the updated component being manufactured using FDM printing.

<img width="260" height="462" alt="b6lit8" src="https://github.com/user-attachments/assets/5ea060c9-dac4-47b5-960f-fa7aa854c842" />


#### 4.3 Completed FDM Print

After printing the updated model, I inspected the physical component and compared it to the previous version. The revised print included the shorter snap-fit section, extended hook connection, and modified triangular geometry.

<img width="224" height="222" alt="Unknown-11" src="https://github.com/user-attachments/assets/afddaf7d-844d-44a3-a31c-1488a0f2ea4f" />

#### 4.4 SLA Hook

I kept the original SLA-printed hook from Part 1 because my main focus was improving the FDM support. I did not redesign or reprint the SLA hook during Part 2. Instead, I modified the FDM component to improve its compatibility with the existing hook.

<img width="301" height="276" alt="Unknown-16" src="https://github.com/user-attachments/assets/1a396174-db97-49e8-ac09-245ba3128d20" />

### 5. Final Prototype Assembly and Testing

#### 5.1 Final Assembly

After manufacturing the updated FDM component, I assembled it with the original SLA hook and installed the prototype on the shower rod. The FDM attachment connects around the rod, while the hook is inserted into the opening in the angled support.

The triangular support compensates for the rod's downward slope, allowing the hook to extend outward and provide a place to hang the loofah.

<img width="470" height="495" alt="Screenshot 2026-11-23 at 11 13 18 PM" src="https://github.com/user-attachments/assets/53590fc3-d2f5-454f-a9aa-bdcd0eba3c7d" />


<img width="398" height="404" alt="Screenshot 2026-11-23 at 11 13 30 PM" src="https://github.com/user-attachments/assets/86c8db87-a861-4797-9b43-1ccf28f2ca24" />


<img width="243" height="265" alt="Screenshot 2026-11-23 at 11 13 48 PM" src="https://github.com/user-attachments/assets/b9ec1e5e-c816-4153-be2c-f9b715cec5a7" />


<img width="248" height="228" alt="Screenshot 2026-11-23 at 11 13 39 PM" src="https://github.com/user-attachments/assets/e411e5cf-703e-4dcc-953c-e509f732b699" />



#### 5.2 Testing Results

The updated prototype was assembled and tested on the actual shower rod with the loofah attached. The final photos show that the revised support can be installed on the rod and that the SLA hook can hold the loofah. The adjustments to the geometry allowed me to assemble the updated support with the original SLA hook. The hook also appears closer to the intended horizontal orientation in the installed side view. Although the prototype demonstrates the intended function, further testing would be needed to determine how securely it remains attached during repeated use and whether the connections maintain their position over time.

### 6. Assembly and Use Instructions

1. Position the FDM snap-fit attachment around the shower rod.
2. Carefully press the attachment onto the rod until it is seated.
3. Insert the SLA hook into the opening in the triangular support.
4. Check that both components are properly connected.
5. Hang the loofah from the hook.
6. Check that the holder remains in place and supports the loofah.

The design can be installed without permanently modifying the shower.

### 7. Final Presentation Preparation

For my final presentation, I prepared a one-slide summary explaining the problem, my manufactured solution, and the improvements made during the design process. The presentation focuses on the angled shower rod, the snap-fit attachment, and how I used FDM and SLA printing to create the prototype.

[Download the One-Slide PowerPoint Presentation](Loofah_Holder_Week2_One_Slide.pptx)

This presentation summarizes the problem, the design solution, the FDM and SLA manufacturing processes, and the improvements made to the final prototype.


### 8. Final Video Presentation

For my final video, I will summarize the entire project, including the original problem, design development, manufacturing processes, and final prototype. The video will show how I used FDM printing to create the attachment and SLA printing to manufacture the hook. It will also explain the improvements I made based on peer feedback and testing.


[Watch Final Project Video](final%20vid.mov)

This video demonstrates my final shower loofah holder, including the design process, FDM and SLA printing, improvements based on peer feedback, and the completed prototype.


### 9. Final Reflection

Throughout this project, I learned how important dimensional accuracy and tolerances are when designing parts that need to connect. During Part 1, I encountered problems with the snap-fit being too tight and then too loose. The connection between the hook and triangular support also allowed movement, preventing the hook from staying in its intended position. After receiving peer feedback, I modified the FDM component by shortening one side, extending the hook connection, and adjusting the triangular cut angle. The final prototype was able to hold the loofah on the shower rod, demonstrating the basic functionality of my design. If I continued improving the design, I would focus on further testing the stability of the snap-fit and reducing any remaining movement between the hook and support. Overall, this project gave me experience using SolidWorks, FDM printing, SLA printing, and the iterative engineering design process to develop a practical solution to an everyday problem.


### SolidWorks Design Files

- [SDP_FD1 – Original FDM Design](SDP_FD1.SLDPRT)
- [SDP_FD2 – Refined FDM Design](SDP_FD2.SLDPRT)
- [SDP_HOOK – SLA Hook Design](SDP_HOOK.SLDPRT)

These SolidWorks files include the original FDM design, the refined FDM design based on peer feedback, and the SLA-printed hook used in the final assembly.

