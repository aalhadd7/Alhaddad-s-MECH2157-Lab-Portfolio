# MEGR 2156 – Final Project (1/2): Shower Loofah Holder

##  Project Overview

For my final project, I designed a removable shower loofah holder that attaches to an existing shower rod. The problem I wanted to solve was not having a convenient place to hang my loofah, which would often fall or take up space in the shower. My goal was to create a holder that could snap onto the rod without drilling holes or making permanent modifications. One of the main challenges was that the shower rod slopes slightly downward, meaning a regular hook would not be positioned correctly. To address this, I designed an angled support that connects the rod attachment to a separate hook. The prototype uses two manufacturing technologies: Fused Deposition Modeling (FDM) for the snap-fit and supporting components, and Stereolithography (SLA) for the hook.

## 1. Research

### 1.1 Spiral Design Process

The Spiral Design Process consists of planning, risk analysis, engineering, and evaluation. Planning involves identifying the problem and determining the requirements. Risk analysis focuses on potential design issues, while engineering involves modeling and manufacturing the prototype. Evaluation involves testing the design and making improvements. I applied this process by measuring the shower rod, designing the components in SolidWorks, manufacturing the parts, and testing their fit. The problems identified during testing will guide my next design modifications.

### 1.2 FDM Anisotropy

FDM printing creates parts by depositing melted material in layers, making the strength of the printed part dependent on its orientation. Parts are generally weaker between layers than within the layers themselves. This is important for my snap-fit attachment because it needs to flex when connecting to the shower rod. I considered the print orientation and wall thickness to reduce the possibility of the snap-fit breaking during installation.

### 1.3 SLA Shrinkage

SLA printing uses resin that is cured using light. The material can experience shrinkage during printing and post-curing, which may affect dimensional accuracy. Since my hook was manufactured using SLA, I needed to consider how dimensional changes could affect its fit within the FDM-printed support. The final assembly showed that the connection had some looseness, indicating that the fitting dimensions still need adjustment. However, I have not confirmed whether SLA shrinkage contributed to this issue.

### 1.4 Laser Cutting Kerf

Laser cutting removes a small amount of material along the cutting path, known as kerf. This must be considered when designing parts that require accurate dimensions or tight connections. One way to compensate for kerf is to create test cuts, measure the resulting dimensions, and adjust the original design. Although I did not use laser cutting for my prototype, understanding kerf is important when designing manufactured parts that must fit together.

## 2. Problem Definition

### Problem 1: No Place to Hang My Loofah

My shower does not have a designated place for my loofah, causing it to fall or take up space. I wanted to create a holder that would keep it hanging securely and make it easier to access.

### Problem 2: Angled Shower Rod

The shower rod is slightly angled downward, making it difficult to attach a hook that hangs in the correct position. This required an additional support component to compensate for the rod's angle.

### Problem 3: Removable Attachment

I wanted a design that would attach directly to the rod without drilling or using permanent adhesives. The attachment needed to be removable while remaining secure enough to support the loofah.

## 3. Problem Selection

I selected the shower loofah holder because it addresses a problem I personally experience. I decided to use a snap-fit attachment that connects directly to the rod, an angled support to compensate for the slope, and a separate hook to hold the loofah.

This project allowed me to use SolidWorks, dimensional measurements, FDM printing, SLA printing, and prototype testing to develop a functional solution.

## 4. Concept Development

### 4.1 Measurements and Initial Design

Before modeling the components, I measured the shower rod to determine the approximate dimensions required for the attachment. These measurements provided a starting point for designing the snap-fit connection.

<img width="434" height="328" alt="Unknown-11" src="https://github.com/user-attachments/assets/15d33e68-0def-4dec-8c00-fa5faf1b1766" />

<img width="434" height="328" alt="Unknown-12" src="https://github.com/user-attachments/assets/6891094f-67d4-4e2b-a5db-db1e141327f2" />


### 4.2 SolidWorks Design Development



I started by designing the snap-fit attachment that would connect directly to the shower rod. I created an angled profile in SolidWorks and used the Thin Extrude feature to give it thickness. The purpose of this component was to allow the holder to attach to the rod without using screws or adhesives.

<img width="875" height="490" alt="Unknown-3" src="https://github.com/user-attachments/assets/a8c0d05a-3647-4639-9a7f-ba0f4b356f35" />

<img width="825" height="602" alt="Unknown-4" src="https://github.com/user-attachments/assets/0b2fa039-6b14-4828-8d6e-c825a01ec61d" />

<img width="208" height="276" alt="Unknown-18" src="https://github.com/user-attachments/assets/dc388cfb-fe20-44da-8bed-aa55ec662d08" />


### 4.3 Hook Design – SDP_HOOK

Next, I designed the hook that would hold the loofah. I created the profile in SolidWorks and used the Boss-Extrude feature to create the solid model. I designed the hook as a separate component so it could be inserted into the support instead of making the entire holder one piece.

<img width="2048" height="820" alt="Unknown" src="https://github.com/user-attachments/assets/08fc063d-ba60-4a66-9c7b-36eebc074c97" />

<img width="2048" height="913" alt="Unknown-1" src="https://github.com/user-attachments/assets/7c40aeed-3abb-44d7-9a92-f750987f0d70" />


<img width="2048" height="1045" alt="Unknown-2" src="https://github.com/user-attachments/assets/9207cef2-3793-42a3-8ae5-30b7b99ea020" />



### 4.4 Design Modifications

The next challenge was correcting the downward angle of the shower rod. I designed an angled support with a triangular section that would allow the hook to sit closer to perpendicular to the floor. I also created a rectangular opening in the support where the hook could be inserted. After reviewing the original design, I modified the support dimensions to improve its geometry and the connection with the hook. I increased one dimension from 1.00 inches to 1.15 inches and another from 0.45 inches to 0.70 inches. I then used additional Cut-Extrude features to create the opening for the hook.

<img width="809" height="512" alt="Unknown-6" src="https://github.com/user-attachments/assets/b2674626-3b33-40de-961c-dff042b7ff65" />

<img width="2048" height="1024" alt="Unknown-7" src="https://github.com/user-attachments/assets/9ac45659-fc0f-409e-a6d2-f443364f8648" />

<img width="2048" height="1107" alt="Unknown-8" src="https://github.com/user-attachments/assets/19159220-22ec-4388-a2e5-965334deff25" />

<img width="2048" height="1040" alt="Unknown-9" src="https://github.com/user-attachments/assets/5c9c40c3-2af0-401a-92b2-6da10cc078b6" />


<img width="849" height="536" alt="Unknown-10" src="https://github.com/user-attachments/assets/97c5894d-eb70-4519-a5de-17d086eb1400" />


### 4.5 FDM Printing

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

### 4.6 SLA Printing

I used SLA printing to manufacture the separate hook component. SLA printing was useful for creating the detailed shape of the hook that would connect to the FDM support. This allowed me to combine two different manufacturing technologies in the final prototype.


<img width="100" height="177" alt="b64j06" src="https://github.com/user-attachments/assets/c8cc9ae5-894a-461d-9221-04a94c252782" />



<img width="301" height="276" alt="Unknown-16" src="https://github.com/user-attachments/assets/36e9d1a6-21e3-4782-a646-fb4dd894c7f7" />



## 5. Prototype Assembly and Testing

After manufacturing the components, I assembled the hook and support and attached the prototype to the shower rod. The holder was able to support the loofah, but testing revealed two problems that still need improvement.

### 5.1 Snap-Fit Connection

The first issue was the snap-fit attachment. My initial fit was too tight on the shower rod. After modifying the design, the connection became too loose. This showed that the attachment dimensions need further adjustment to achieve a secure fit while still allowing the holder to be removed. I also thought it was too long for no reason so I decided to shorten it. 

<img width="309" height="218" alt="Screenshot 2026-11-17 at 4 39 17 PM" src="https://github.com/user-attachments/assets/3262173f-ac07-434d-b699-46d71c890bad" />



### 5.2 Hook Connection and Alignment

The second issue was the connection between the hook and the angled support. Although the hook fits into the opening and can hold the loofah, the connection is not tight enough to maintain the intended perpendicular position consistently. To fix this, I would need to adjust the dimensions of the rectangular opening or the connecting section of the hook to reduce movement between the parts.

### 5.3 Final Prototype Testing

Despite these issues, the assembled prototype demonstrated that the general design can hold the loofah on the shower rod. The remaining improvements involve making both connections more secure and maintaining the correct hook orientation.

<img width="328" height="268" alt="Unknown-19" src="https://github.com/user-attachments/assets/cd1ccb67-c691-4c81-9cbd-9944e52ac4e5" />


## 6. Project Video Presentation

I recorded a video explaining the problem and how my prototype was designed to solve it. The video explains why I needed the holder, how the angled shower rod influenced the design, and how the printed components connect to support the loofah.

https://github.com/user-attachments/assets/fd4ed841-db2d-40ce-a4b7-f1e961264ac5

## 7. Documentation 

In the early phases of projects I like to do a scrape brain dump on a piece of paper so that I can start visualizing what I want to design and what I would need to design it. I like to make little notes such as "get in." so that I can remember to measure my parts for example. It is definitely a my eyes only type of work as it is very informal and simply for mental clarification.

<img width="461" height="543" alt="Screenshot 2026-11-17 at 4 32 27 PM" src="https://github.com/user-attachments/assets/14dad12d-86bc-4648-a383-b7ff57ec2c67" />


## Reflection and Future Improvements

Throughout this project, I learned how important dimensional accuracy and tolerances are when designing components that fit together. Although the prototype was able to support the loofah, the connections were not as secure as I originally intended. The snap-fit attachment went from being too tight to too loose, showing that small dimensional changes can significantly affect the fit. I also learned that designing an angled support does not automatically guarantee the hook will remain perpendicular if the connection between the parts has too much clearance. For my next iteration, I would focus on adjusting the snap-fit dimensions and improving the connection between the SLA hook and FDM support. I would then test the revised prototype to determine whether the holder remains stable and maintains the correct alignment.

Overall, this project gave me experience using two different 3D printing technologies and applying an iterative engineering design process to solve a real-world problem.
