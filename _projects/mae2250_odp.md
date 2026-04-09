---
layout: project
title: MAE2250 Open Design Project
description: [none]
technologies: [none yet]
image: assets/images/Capture d’écran 2026-04-09 à 11.54.07.png
--- 

[put project context here]

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

## Proposed direction(s)

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
## Design Tests

## Success Criteria


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

--- 

# Client Report

