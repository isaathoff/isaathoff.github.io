---
title: Nonthermal X-ray Properties of Rotation-Powered Pulsars and their Wind Nebulae - Notes on Li, Lu & Li 2008
date: 2023-10-06 01:00:00
categories: [Papers]
pin: false
image: /img/20231006-RPPs-PWNe-archive.png
tags: [x-ray, pulsar, rotation-powered-pulsar, pulsar wind nebulae (PWN), XMM-Newton, Chandra]
---

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

## Studying rotation-powered pulsars and pulsar wind nebulae with XMM-Newton and Chandra
The paper ["Nonthermal X-ray Properties of Rotation-Powered Pulsars and their Wind Nebulae"](https://arxiv.org/abs/0707.4279) by Li, Lu & Li 2008 studies 27 rotation-powered pulsars and 24 pulsar wind nebulae using XMM-Newton and Chandra. The high spatial resolution of these instruments allows them to see the pulsars and their pulsar wind nebulae separately. They then look at the luminosities (X-ray) and spectra and analyse them to see if there are any interesting correlations between luminosity, spin-down power, characteristic age, etc. The conclusion of the paper is that the particle wind model (where X-ray emitting electrons are accelerated by the termination shock of the wind) seems to be in agreement with the statistical study of the spectral properties of the pulsar wind nebulae.


### What are rotation-powered pulsars?
Rotation-powered pulsars are fast-spinning, highly magnetized neutron stars that emit radiation powered by their rotational energy. These objects can be observed in X-rays and their emission can contain both thermal and non-thermal components:
- The thermal component can be pulsed or non-pulsed.
    - The non-pulsed component comes from the whole pulsar surface and has a temperature of about 0.1 keV.
    - The pulsed component comes from hot spots with temperatures of about 1 keV. These hot spots are heated by relativistic particles from the magnetosphere flowing back to the surface and hitting it. 
- The non-thermal emission comes from the pulsar's magnetosphere and can also contain pulsed and non-pulsed components.

Sometimes there is a pulsar wind nebula surrounding these rotation-powered pulsars, and its X-ray emission is non-pulsed and can often dominate the non-thermal emission of the system.

In order to better understand these systems, statistical studies have been carried out, and they find many different correlation properties, such as
- $$L_X \propto \dot{E}^{1.39}$$, 0.2 - 4.0 keV,
- $$L_X \approx 10^{-3}\dot{E}$$, 0.1 - 2.4 keV,
- $$L_X \propto \dot{E}^{3/2}$$, 2 - 10 keV,
- $$L_X \propto \dot{E}^{1.34}$$ ,
- $$L_X^\text{pul} \propto \dot{E}^{1.2}$$ ,
- $$L_X \propto \dot{E}^{1.15}$$ (model),
- $$L_X^\text{npul} \propto \dot{E}^{1.4}$$ (model).

However, the problem is that the detectors used in these studies have relatively low spatial resolution, and the emission from the pulsar and the surrounding pulsar wind nebula can be difficult to separate. This is addressed and improved in the current paper.

### How did they process the data from their pulsars?
The primary instrument they used was Chandra, in particular the Advanced CCD Imaging Spectrometer (ACIS) in Timed Exposure mode, which can spatially resolve pulsars from the surrounding nebula. The data are then calibrated with CIAO and CALDB, charge transfer inefficiency effects are corrected, the background is cleaned, and afterglow is removed. Time intervals with strange background rates are rejected in a next step. Then the positions of the pulsars are obtained and the spectra are fitted using XSPEC (with a power-law and a power-law+blackbody model).

Furthermore, the $$N_H$$ was determined for different pulsars in different ways (e.g. from spectral fitting, joint fitting, or literature), as well as the distances (radio dispersion measurements, literature, LMC value). This allows the spectra to be fitted and the luminosity to be determined ($$L_X = 4\pi d^2 f_X$$).

### What do they find?
This paper uses Chandra, XMM-Newton 2 - 10 keV, nonthermal X-ray fluxes and spectra. With that, they find
- $$L_X^\text{psr}$$ and $$L_X^\text{pwn}$$ are strongly correlated with $$\dot{E}$$ and $$\tau$$
- $$L_X^\text{psr}$$ shows a weaker correlation with $$P$$ and $$\dot{P}$$
- $$L_X^\text{pwn}$$ shows a similar weak correlation with $$\dot{P}$$ only
- $$\Gamma^\text{pwn}$$ is positively correlated with $$L_X^\text{pwn}$$
- Pulsar wind nebulae $$L_X$$ is 1-10 times larger than that from the underlying pulsar
- Pulsar photon index: 1 - 3

The final conclusion of this paper is that the spectral properties of the pulsar wind nebula are consistent with the particle wind model.