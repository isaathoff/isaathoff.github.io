---
title: Search for faint transients with XMM-Newton. Four new extragalactic Type I X-ray bursters - Notes on Pastor-Marazuela et al. 2020
date: 2023-10-10 01:00:00
categories: [Papers]
pin: false
image: /img/20231010-EXOD-Transient-Burster.png
tags: [x-ray, EXOD, XMM-Newton, Type I X-ray burster]
---

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

## The Idea
XMM-Newton's standard pipeline determines the variability of sources that are bright enough with $$\chi^2$$ and fractional variability tests. The problem is that faint sources that are transient on short timescales are missed by these tests. This paper, with the title ["The EXOD search for faint transients in XMM-Newton observations: Method and discovery of four extragalactic Type I X-ray bursters"](https://arxiv.org/abs/2005.08673) addresses this problem and presents EXOD: The EPIC-pn XMM-Newton outburst detector algorithm. By applying this algorithm to about 5700 observations, they find 2500 variable sources, of which 35 have not been previously classified. These include stellar flares, AGN, and four extragalactic Type I X-ray bursters in M31. These are neutron star low-mass X-ray binaries, and their detection has doubled the number of known neutron stars in M31.

### The Context
Compared to the static sky, the authors of this paper note that the dynamic sky is relatively unexplored. Although there have been some efforts to add variability information to the XMM-Newton catalogue, for example, it still leaves a lot to be desired. Here, a new algorithm is developed that aims to add more variable sources to the catalogue. The algorithm is called EXOD: the EPIC-pn XMM-Newton Outburst Detector. It is designed to detect fast and faint (<100 counts) transients by computing the variability of each pixel from each observation. The steps are
1. Extract the time and pixel of arrival of each event detected during the observation from the event file.
2. Photons in a 3x3 square around each pixel are then summed to increase the signal-to-noise ratio and reduce the stochastic variability.
3. Events per pixel are binned into time windows (TW), which is an input to the algorithm.
4. The GTI file is read.
5. A good time ratio of each time window is calculated (GTI duration divided by total TW).
6. The counts per TW are divided by the good time ratio. Only results above a threshold are taken into account.
7. The variability is calculated for each pixel based on the maximum and minimum number of counts per TW and the median number of counts.

By applying the EXOD to the XMM observations, they find that the algorithm picks up a wide variety of variable phenomena. The sources have different variability timescales (long and short flares), can be periodic or aperiodic, and have different rates of rise and fall. And they correspond to a number of different classes, such as 
- Ultra-compact binaries
- High proper motion stars with flares
- Supergiant fast X-ray transients with aperiodic flares
- Beta Lyr eclipsing binaries
- Magnetic cataclysmic variable
- Low mass X-ray binary with eclipse and type I X-ray burst

### The Unknown Sources
Using their method, the authors find 26 unidentified sources and a further 9 sources in M31 that were detected but not flagged as variable. They examine each of these in turn. Two sources were also found by Alp & Larsson 2020 and appear to be supernova shock breakouts, possibly from blue supergiants. The authors of this paper see this as a confirmation of the potential of EXOD to identify transients.

### Follow-up
Something I would like to follow up on is the comment that some papers have used machine learning algorithms where timing parameters are the main classification feature. See Lo et al. 2014 and Farrell et al. 2015.