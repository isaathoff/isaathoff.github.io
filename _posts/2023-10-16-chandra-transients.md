---
title: Extragalactic fast X-ray transient candidates discovered by Chandra - Notes on Quirola-Vásquez et al. 2022
date: 2023-10-24 01:00:00
categories: [Papers]
pin: false
image: /img/20231016-chandra-transients.png
tags: [x-ray, transient, Chandra]
---

Link to paper: ["Extragalactic fast X-ray transient candidates discovered by Chandra (2000–2014)"](https://arxiv.org/abs/2201.07773) 

## Searching for fast X-ray transients
Fast X-ray transients are sources that show flashes of X-ray emission lasting from a few minutes to hours. The origin of these flashes is still unknown, in part because we can't find clear multi-wavelength counterparts. In this paper, they go through the Chandra source catalogue to look for more sources and include multi-wavelength data to ensure that they are looking only at extragalactic sources.

There are a number of simple criteria that must be met for the source to be found as a transient candidate in their algorithm. These criteria must all be met:
1. The total number of counts is greater than the 5 sigma Poisson upper limit of the background counts.
2. Two halves of the light curve (first and last, or shifted to the end and middle of the observation) must be statistically different at a 4 sigma significance level.
3. One half of the observation must have at least 5 times the counts of the other half.

Interesting fact: One advantage of using Chandra is the low average number of background counts, which allows the detection of transients with only about 10 total counts.

### Narrowing down the sources
After applying the algorithm, they narrow down the more than 200,000 sources to about 700 fast X-ray transients. This is followed by further selection:
1. Using archival X-ray data, they made sure that the source was not detected in earlier and later X-ray observations. (They explain many details for these steps, which I will skip here, see section 2.5.1.ff.). After this step, 170 candidates remain. 
2. They also search for optical detections in Gaia, which leaves 274 sources. Together with the first step, this leaves only 63.
3. Using NED, SIMBAD and VizeR, more Galactic and Local Group objects are filtered, leaving 203 sources, and together with the first and second steps there are 29 candidates.
4. Some sources are found in galactic nebulae with point-like NIR counterparts, and some have been found as stars in Hubble Space Telescope images. There are 20 candidates remaining.
5. Finally, some observations are affected by background flares, leaving 14 sources as candidates for fast X-ray transients.

Of these candidates, five have been previously detected as fast X-ray transients, and a further six have been detected but not properly characterised. Three of the candidates have previously been classified as high-mass X-ray binaries, but they remain in the sample for consistency.

### Spatial, temporal and X-ray spectral properties 
The remaining 14 fast X-ray transient candidates are then examined in detail for their spatial, temporal and spectral properties. I will only highlight a few things I noticed while reading, as it is a very thorough analysis:
- The sample of sources is randomly distributed over the Chandra CSC2 observations of the sky.
- The light curves of 6 of the candidates are well described by broken power law models. Two are explained by simple power-law decays. Some show multiple flares, some don't.
- For the spectra, they tried three models: an absorbed power law, an absorbed thermal bremsstrahlung model, and an absorbed blackbody model. This is because they do not know the origin and the processes of these sources, but at the same time more complex models cannot be used because of the limited number of detected counts. Using these models, the authors find different parameters, such as the photon index and black body temperatures.
- They think that there are indeed two different populations in fast X-ray transient sources, local and distant.
- They also speculate about the candidates, but say that it's probably a heterogeneous group, since they have such different properties.

### Some final remarks
- From the initial 200,000 X-ray sources, 14 fast X-ray transients are identified in this paper. These candidates have peak fluxes in the 0.5-7 keV energy range between 10^-13 and 10^-10 erg cm-2 s-1. Their durations range from 4 to 40 kiloseconds. Five of the events are associated with local galaxies, seven are more distant (more than 100 Mpc). 
- It is difficult to determine the origin and nature of these objects, the distances are difficult to determine, and the host properties leave many questions unanswered.
- In the future, more recent optical and NIR observations should be used to find the host galaxies and better constrain their energetics. 

### Note
- For low counts per bin, the maximum likelihood statistic for a Poisson distribution should be used: the Cash statistic (C-stat, C = -2lnL+const.). Chi-square cannot be used for goodness of fit, instead the Bayesian X-ray Astronomy (BXA) package can be used, using Monte Carlo nested sampling.