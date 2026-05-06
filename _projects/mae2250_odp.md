---
layout: project
title: MAE2250 Open Design Project
description: [none]
technologies: [none yet]
image: assets/images/Capture d’écran 2026-04-09 à 11.54.07.png
--- 

This project is part of the core design assessment for the Mechanical Engineering curriculum at Cornell University, where student teams apply the full engineering design process to a real-world, stakeholder-driven problem. Conducted within the MAE2250 course, the project emphasizes translating user needs into functional requirements, generating and evaluating concepts, and developing a validated proof-of-concept prototype.

Our team, Vine Vanguard, is collaborating with partners including Cornell CALS Extension, E&J Gallo Winery, and National Grape Cooperative Association to address an agricultural challenge affecting vineyards across New York State. These stakeholders bring both technical expertise and lived experience, ensuring that proposed solutions are grounded in real vineyard workflows and constraints.

Within the scope of the course, the team is responsible for defining engineering specifications, iterating on mechanical concepts, and delivering a functional prototype by the end of the semester. The project prioritizes scalability, reliability, and integration into existing vineyard practices.

# Project Contents
- [Client Pitch](#client-pitch)
- [Functional Prototype](#functional-prototype)
- [Client Report](#client-report)

--- 
# Client Pitch

**Team:** Vine Vanguard  
**Client(s):** Cornell CALS Extension / E&J Gallo Winery / National Grape  

## Problem statement

Vineyard owners across New York State are affected by the rapid proliferation of Spotted Lanternflies (SLF), which lay egg masses directly on grapevines and nearby surfaces. They are trying to reduce SLF reproduction by destroying egg masses before they hatch. Each female SLF lays 30-120 eggs per year, and heavily infested vineyards can have 400 SLF per vine. This means that eggs are being laid exponentially. Current elimination methods such as crushing egg masses one-by-one is ineffective if they are not fully destroyed, and experimental ovicides kill only up to 75% of eggs (Krawczyk). Even a single surviving egg mass can enable SLF persistence, escalating plant damage and contaminated harvests.
  

## Impact
A scalable, systematic method for eliminating large quantities of SLF egg masses is necessary to meaningfully reduce infestations and prevent substantial economic losses for vineyards. Without effective, large-scale intervention, projected losses in the Lake Erie and Finger Lakes regions alone could reach approximately $8.8 million within three years (Gómez, 2025), highlighting the urgent need for proactive and reliable egg-destruction strategies. 

## Proposed directions

**Mobile Composting Crusher**
A mobile crushing and composting unit designed to move through vineyard rows, collect scraped masses, crush and store remains for compost use. 
Handles large quantities of eggs, and will be equipped with multiple contingency mechanisms to crush 100% of input masses.
End-of-semester proof-of-concept: A scaled prototype of the crushing and collecting mechanism, along with basic mobility to drive through vineyard rows.

**Egg Crusher Attachment**
A small, lightweight crushing attachment to integrate with other systems that crush SLF eggs, such as an autonomous drone
End-of-semester proof-of-concept: A prototype of a compact crushing mechanism that can be mounted onto a flat surface (or future device), and operate while inverted. 

## Key risks / unknowns

- Additional operating considerations to prevent interference with harvesting equipment.
- Ensuring 100% destruction of egg masses metric is met, preventing accidental redistribution.
- Our design assumes the ‘scraping’ step of egg mass removal has already been completed, as we chose to focus on the crushing and disposal stage.

## Questions for the client
Focus on questions they can answer from lived experience.
1. **Is a solution that reincorporates crushed egg waste into the vineyard as compost appealing?**  
   *Decision affected:* This would impact potential usage of chemicals to eliminate the egg masses.
2. **What is your actual and ideal egg removal rate, per day and/or per acre?**  
   *Decision affected:* This would allow us to create optimal crushing speed settings.

--- 

# Functional Prototype
## Design Documentation
![parts list](image path)

![prototype 1 dissassembled](assets/images/prototype 1_parts.png)
![prototype 1 assembled](assets/images/prototype 1_assembled.png)

## Design Tests

### Test 1: Does the device’s assembly of press-fits remain intact during use?

**How this was tested:** Completely construct device in accordance with intended assembly, including the insertion of the grid mesh, while noting any times where excessive force was required to connect parts. Firmly shake the device for 10 seconds, in upright and inverted positions. Inspect the entire device for any loosened or detached components.

**Results:**
- Primary Construction: The press-fits for the shaft-spiral and housing-funnel connection were securely fastened without excessive force. The tolerances for the connections between the housing top and bottom were inaccurate, and the two could not be press-fit together. Extra adhesion (duct-tape) was required to secure these two components. The mesh was secured easily into the housing groove. 
- Post Shake Test: No loosen pieces were found in the device. The connected shaft and spiral slid in and out of the housing bottom when inverted. 

**Required Changes:** In next prototypes, we will alter the CAD geometries for the housing components so that they securely connect via press-fit. 

### Test 2: Does the spiral properly rotate without jamming/getting blocked in its motion? 

**How this was tested:** Rotate the device manually through multiple full crushing cycles including before, during, and after the insertion of model egg masses (hydrated Orbeez). Observe whether or not the spiral experiences any resistance, blockage or misalignment during rotation. Testing was conducted over varying loads (no Orbeez, 20-30 Orbeez, 50 Orbeez) to simulate realistic operating conditions.

**Results:**
- Rotation Without Orbeez: The spiral rotated smoothly, with minimal resistance and no visible wobbling or misalignment of the shaft within the mesh housing. 
- Rotation With Orbeez (during operation): Rotation became inconsistent once Orbeez were introduced. Some Orbeez became lodged beneath the spiral rather than being carried through the crushing mechanism. This created intermittent resistance and slight jamming. Additionally, it prevented many Orbeez from being fully crushed since there was no resistance between the spiral, the Orbeez, and the mesh. 
- Mesh Interaction: Due to unforeseen ordering complications, we used a temporary replacement mesh for testing in our lab section. The openings of this replacement were approximately 8mm in diameter, while our partially hydrated Orbeez were about 3mm in diameter. This meant the Orbeez could simply fall through the mesh rather than being crushed against it by the spiral. We tried to rectify this by adding multiple layers of mesh in the housing to create smaller openings, but Orbeez would still fall through. Due to this large mesh opening size, during our prototype testing, Orbeez were not properly supported during rotation, further contributing to slipping and inconsistent contact with the spiral.

**Required Changes:** 
In next prototypes, we will add a guide or mechanical restraint such as little arms attached to the inside columns of the mesh housing to keep the spiral flush against the bottom of the mesh housing. This will prevent eggs from being trapped underneath and remain uncrushed during rotation. Additionally, as we originally planned, we will replace the temporary replacement mesh with much finer mesh to prevent Orbeez from slipping through the openings.  
 
### Test 3: How efficient is the juicer inspired mechanism at crushing the egg masses? What percentage of eggs come out of the device entirely crushed?

**How this was tested:** Insert a standardized number of Orbeez (model SLF eggs) into the device. Manually crank the spiral shaft to engage the crushing mechanism for ~30 seconds. Divide the number of eggs that come out intact by the number of eggs inserted into the device. This will give us the percentage of eggs that were not destroyed. Repeat this process for numerous trials and average the percentages.

**Results:**
As stated in Test 2, the inaccurate sizing for the replacement mesh meant that our trials did not produce crushed Orbeez. However, the trials allowed us to examine the model eggs’ motion throughout the crushing process. 
- Spiral Design: We observed that the spiral’s egg-like shape, which tapered out to the diameter of the housing mesh groove then tapered in, allowed Orbeez to accumulate at the housing bottom. The current design had no method to move the settled eggs outside of inverting the device.
- Mesh Stability: The interactions between the spiral and the mesh were observed. We suspect that the mesh will not be stable enough in the groove to withstand the lateral load of eggs pushed into it by the spiral at regular operation.

**Required Changes:** 
To address the accumulation of Orbeez at the housing bottom, the spiral will be redesigned to not taper in towards its base. Adjustments to the mesh will be explored to make it more secure against the eggs pressing against it. Configurations such as a 3D printed cylinder with cutouts for mesh pieces, a 3D printed cylinder with an embedded mesh design, and a solid cylindrical column with internal sandpaper lining may be tested.

## Success Criteria
This project focuses on designing a device attachment that integrates with an existing scraping process to mechanically crush Spotted Lanternfly (SLF) egg masses immediately after removal, ensuring they do not hatch. Success will be evaluated based on effectiveness, processing speed, and appropriate sizing.

### Criteria 1: Egg Crushing Effectiveness
**What it assesses:** the ability of our mechanism to completely and reliably crush inserted masses

**Metric:** ~80% eggs crushed per egg mass

**How it will be measured:**  Insert a standardized number of Orbeez into the device and run the crushing mechanism for a standardized amount of time. After each trial, count total Orbeez inserted and crushed Orbeez after being run through the mechanism. Calculate (crushed/total) x 100 to get the percentage of eggs crushed.

**Exhibit-Day demonstration:** Live crushing of Orbeez demo; Calculate crushing efficiency in real time for observers

### Criteria 2: Processing Rate (eggs per second)
**What it assesses:** speed at which device crushes a desired amount of eggs

**Metric:** Assume it takes ~10-20 seconds to hand-scrape an SLF egg mass from an uneven surface and insert the masses into the device’s inlet funnel. Since there are approximately 30-50 eggs per egg mass, we’d want to crush the eggs in the same timescale at which they’re being inputted into the mechanism. So, taking the upper limit, we’d hope to crush 50 eggs in 20 seconds, translating to a processing rate of around 2-3 eggs per second.

**How it will be measured:**  Insert 50 Orbeez into the device. Turn the crushing mechanism on for 20 seconds. Count the number of crushed eggs produced and divide by the processing time to calculate the processing rate. Repeat this process for multiple trials and average. 
Repeat this trial for greater quantities of eggs over a standardized amount of time. Count the number of crushed eggs produced and calculate the processing rate. Compare to the desired 2-3 eggs per second metric.

**Note:** This would not be tested with our manually controlled prototype, but will be tested when we integrate an electric motor into the device.

### Criteria 3: Device size and weight
**What it assesses:** practicality for attachment and field use

**Metric:** For our device to be easily attachable, we’d want to make it small and lightweight. Based off sizes of common juicers and electric grinders, as well as accounting for the size of the motor we hope to incorporate into the device, we hope to create a device whose bounding box is less than or equal to 6x6x10 inches
The mechanism is intended to be attached to another device’s frame reasonably. Thus we will base the ideal weight on regular handheld devices such as a computer, making the maximum weight to be 4lbs

**How it will be measured:** After creating our next prototypes, physically measure the size of device using rulers or calipers; Measure the weight of the device using a scale


--- 

# Client Report
## Problem Statement and Context

Vineyard owners across New York State are affected by the rapid spread of Spotted Lanternflies
(SLF, whose presence in the Lake Erie and Finger Lakes regions alone could have projected losses reaching approximately $8.8 million within three years [1]. A single SLF egg mass contains 30-50 eggs, and populations can spread rapidly across large areas of vineyard land. To effectively address this spread, reduce proliferation, and prevent these economic losses from spreading to other parts of the nation, these invasive insects should be targeted while in their egg stage. Destroying eggs prevents the flies from maturing into reproductive adults, reducing the number of SLF that will lay future egg masses and limiting their exponential population growth. Our team focused on developing a mechanical solution for large-scale egg mass destruction that can be deployed at the vineyard level.
Current elimination methods are not suitable for addressing large-scale SLF populations.
Manually crushing individual egg masses is time-consuming and inconsistent. Submersion into rubbing alcohol requires constant refilling and storage capacity. Experimental oil ovicides are only effective on 75% of eggs [2]. Additional consideration must be given to the consequences of ineffective elimination, as even one surviving egg mass can enable SLF persistence, escalating plant damage and contaminated harvests.
There is a need for a systematic method for eliminating large quantities of SLF egg masses that can be integrated into existing collection workflows. This method must be consistently effective, practical for real-world use, while minimizing storage, disposal, and labor demands on vineyard operations during implementation.

## Final Prototype and Application
We developed a device that mechanically crushes eggs, utilizing a juicer-inspired crushing mechanism.
How it works:
- Eggs masses enter the mesh cylinder chamber through an inlet funnel.
- A rotating spiral, driven by an electric motor, transports the egg masses downward while simultaneously pressing the eggs against the mesh cylinder, where the crushing occurs.
- A sweeper attached to the rotating spiral pushes crushed eggs towards a hole in the bottom of the mesh housing, falling out of the device through an outlet funnel.
This device will be deployed in the field alongside the given collection method that best suits the vineyard's needs, such as a manual scraper or an autonomous scraping robot. The device is modular, such that its method of accepting and ejecting egg masses can be easily changed

## Conclusion and Reccomendation
We would recommend the continued research and development of the Egg Crusher for applications in vineyards. The device in its current form is a successful proof of concept for a scalable, efficient, and practical egg extermination method, demonstrating basic mechanical motion. Its ~80% crushing efficiency is on par with current methods, without the drawbacks of consistent maintenance or manual labor. Additionally, its 100% efficiency for ejecting crushed eggs of a standardized diameter suggests the crushed eggs can be re-incorporated into the ecosystem as a compost ingredient if desired by the vineyard owners.
We would suggest three primary redesigns in future phases of this project:
1. Spiral and sweeper geometry. Pitch angle, spiral diameter, and other features can be optimized to
Features can be optimized 1o
improve crushing efficiency and properly push the crushed eggs towards the outlet funnel.
2. Compactness. The system can be scaled down to reduce weight and improve portability, making it easier to deploy in the field alongside a collection device.
3. Contingency mechanisms. Incorporating multiple built-in crushing mechanisms arranged in a linear series can improve crushing efficiency, as eggs not crushed by the first spiral will be crushed by the second crushing mechanism right below.

