---
title: Extragalactic transient candidates, 2nd Swift-XRT Point Source catalogue - Notes on  Eyles-Ferris et al. 2022
date: 2023-10-25 01:00:00
categories: [Papers]
pin: false
image: /img/20231025-transients-Swift.png
tags: [x-ray, transient, Chandra]
---

Link to paper: ["Extragalactic transient candidates in the Second Swift-XRT Point Source catalogue"](https://arxiv.org/abs/2207.04067) 

## Transient candidates with Swift-XRT
The Neil Gehrels Swift Observatory X-ray telescope (Swift-XRT) provides an excellent opportunity to study extragalactic transients due to its combination of good sky coverage and sensitivity in the 0.3 to 10 keV energy band. In this paper, the second Swift-XRT point source catalogue is used to search for transients that have not yet been found. 

### Source samples
The entire catalogue consists of more than 200,000 sources. Since only extragalactic transients are of interest, only sources in the vicinity of known galaxies are selected. The sample is divided into an inactive host sample and an active host sample - simply indicating whether the host galaxy is inactive or has an active galactic nucleus.

The selection is based on several steps. The first step is a quality cut using one of the flags in the catalogue:
- From the initial >200,000 sources, about 160,000 are left.

Let's focus on the active host sample first. There are two ways to add a source to the active host sample: the first is by cross-matching with the SDSS Quasar Catalogue. The other way is by checking the hosts and their activity. 
- Combining the two results in just under 18000 sources being added to the Active Host sample.

The Inactive Host sample is created using only the host check and the host activity check. 
- Just under 13000 sources are added.

The remaining sources - those that fail the quality cut and have no host galaxy identified alongside them - are discarded. This is by far the largest part of the sample, with 175,000 sources. This is to be expected, since most of the sources in the catalogue are likely to be stellar sources within the Milky Way.

### Flares
Based on the two samples, sources that appeared to be flaring were selected. This was done in two ways: by inspecting the XRT light curves and by cross-checking with external catalogues. 

For the light curves, the observed count rates were converted to fluxes using the PIMMS tool and assuming a power-law spectrum with index 1.7, which is typical for AGNs. The host column density was set to a mean value for the Milky Way column density and, if not known, the redshift of the source was set to the mean value of its sample (active and inactive). The ratio of the peak flux to the mean flux was then determined and a cut-off value was set to separate flaring from non-flaring sources. For the light curves they set this to 25, but later for the catalogue it is lower, at 10. From the light curve data, 110 and 31 sources were found to be flaring in the inactive and active hosts respectively. Together with the cross-matching with other catalogues, a total of 334 sources in inactive hosts and 372 sources in active hosts were selected.

### Classification of the candidates
Candidates were classified as follows:
1. Spurious flares (e.g. caused by pileup or Eddington bias)
2. Galactic sources (only four were found by checking SIMBAD, suggesting that the selection criteria worked well)
3. AGN
4. Known transients
5. New Candidate Transients (19 found)

### Characterisation of the 19 new candidates
10 of the 19 sources do not have enough counts to fit their spectra. Therefore not much can be said about them. The remaining "bright" sources will be studied in more detail. The spectra have been fitted with a power law and APEC (Astrophysical Plasma Emission Code), as well as a blackbody model. The power laws are representative of AGN or GRBs, while the APEC model describes shock-heated plasmas found in dark matter haloes or the inner regions of black hole accretion disks. The blackbody model may be more typical of transients such as tidal disruption events. 

It seems that all the candidates fit reasonably well with all the models, according to the chi-square values (but doesn't that mean that we just can't tell them apart and therefore they mean nothing?) Four of the sources fit best with power laws, two with APECs and one with blackbody. The other two fit two of the models equally well.

Taking them all together, the photon index is consistent with sources such as AGN or GRBs, as well as high-mass X-ray binaries. The APEC model implies higher temperatures than usual for AGN, and the blackbody temperatures are higher than classes such as tidal disruption events. The authors conclude that the majority of candidates are therefore unlikely to be thermally dominated. 

For four sources there was enough data to fit spectra for different epochs. For two of them, the fits are consistent with only small variations, and for the other two, the uncertainty in the parameters was too large to go into more detail.

More observations are needed to better understand these sources.
