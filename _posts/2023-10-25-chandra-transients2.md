---
title: Extragalactic fast X-ray transient candidates discovered by Chandra - Notes on Quirola-Vásquez et al. 2023
date: 2023-10-25 01:00:00
categories: [Papers]
pin: false
image: /img/20231025-chandra-transients.png
tags: [x-ray, transient, Chandra]
---

Link to paper: ["Extragalactic fast X-ray transient candidates discovered by Chandra (2014–2022)"](https://arxiv.org/abs/2304.13795) 

See also the related blog post on the previous paper ["Extragalactic fast X-ray transient candidates discovered by Chandra (2000–2014)"](https://isaathoff.github.io/posts/chandra-transients/)

## Extragalactic fast X-ray transients (FXTs)
Extragalactic FXTs are short (minutes to hours), non-repeating flashes of X-rays (0.3-10 keV) of unknown origin. There are some ideas about the origin of FXTs, such as
1. stochastic outbursts associated with X-ray binaries in nearby galaxies (including ULXs, SGRs, AXPs),
2. X-ray emission from shock breakouts of core-collapse supernovae,
3. off-axis gamma-ray bursts
4. tidal disruption events 
5. binary neutron star mergers.

In the previous [paper (link to post)](https://isaathoff.github.io/posts/chandra-transients) by the same authors, they devised an X-ray flare search algorithm and looked at multi-wavelength constraints to find 14 FXT candidates. Their T90 values range from 4 to 48 ks and the sample can be divided into six "nearby" FXTs with distances less than 100 Mpc and eight distant FXTs with redshifts greater than 0.1. Repeating FXTs are not part of the current paper.

### Sample selection
The first step was to create a source catalogue based on the Chandra observations. This can be done using the CIAO source detection tool wavdetect. This catalogue can then be run through the pipeline to detect transients, as they had done in their previous paper. This involves some light curve splitting and calculation of the total and background counts. If certain criteria are met, the source is added or discarded as a transient. 

Since this method does not ensure the unambiguous identification of true extragalactic FXTs, additional criteria are required. First, non-detection in previous and/or subsequent X-ray observations is important. 98 candidates fulfil this criterion. Second, to rule out a galactic origin related to bright stars, the Gaia catalogue is searched. 68 sources fulfil this criterion. A total of 42 candidates pass both criteria. Third, NED, SIMBAD and VizieR are searched for counterparts. 76 FXTs pass this criterion, leaving a total of 9 candidates. After confirming that none of these are associated with stellar sources, some visual and variability checks are performed and one source does not pass these checks. This leaves a final sample of eight FXT candidates. Three of these have already been discovered and classified as FXTs. 

All candidates are then scrutinised, and a multi-wavelength analysis from radio to gamma-ray is used to search for a companion and host galaxy. Four of the eight FXT candidates have a high probability of association with extended sources. One has too high a positional uncertainty to find an optical or NIR counterpart. Two others have no optical or NIR sources. None of the candidates appear to be in a nearby galaxy within 100 Mpc. 

### Notes on spatial, temporal, X-ray spectral properties and more
- Spatial: Since the FXT candidates are extragalactic and from large distances, and given the isotropy of the Universe on large scales, the distribution across the sky should be random - and this is what they find. 
- Temporal: They also look at the light curves and fit power-law and broken power-law models to them, then use the Bayesian Information Criterion (BIC) to compare the two. Five sources require a break time, three do not. 
- Spectral: An absorbed power-law model is fitted to the data because the origin and processes behind the emission of the FXTs are unclear. This fits the data well with a median slope of 2.6 (range 2.1-3.4 with an outlier at 6.5).
- Two FXTs are aligned with extended objects, supporting an extragalactic origin. Four FXTs could be associated with hosts, supporting an extragalactic origin.
- Three FXTs are incompatible with stellar flaring episodes of galactic M dwarfs and brown dwarfs. Two of them are inconclusive with the present data.
- Although they found in their previous paper that the candidates could be divided into local and distant populations, the present set does not find the same - there are no local FXTs among them. 
- The rate of FXT is about 46 per square degree per year. This is in agreement with other work. 
- The X-ray luminosity function shows that the rate decreases with increasing X-ray luminosity.
- The host galaxies cover a wide range of redshifts (0.3-1.5), stellar masses and star formation rates.
- Several possible origins for the FXTs are discussed, including shock breakouts, gamma-ray bursts, and tidal disruption events. Given the wide range of properties, the FXTs are likely to have a mixture of origins, but it is difficult to pinpoint the exact origin from the data available.

