---
title: Paper published!
date: 2024-03-14 01:00:00
categories: [Papers]
pin: true
image: /img/20240314-pcva.png
tags: [nmf, pcva, pulse profile, pulsar, Cen X-3, RXTE, x-ray, x-ray pulsar, neutron star]
---

My paper on the topic of my PhD thesis is now published! You can find it on the website of the journal Astronomy & Astrophysics here: [Blind source separation for decomposing X-ray pulsar profiles. Introducing phase-correlated variability analysis (PCVA) with a case study of Cen X-3](https://www.aanda.org/articles/aa/abs/2024/03/aa47432-23/aa47432-23.html).

Let's decipher the somewhat cryptic title. Neutron stars form at the end of a massive star's life. After it explodes in a massive supernova, this neutron star is the core that remains, and it can have huge magnetic fields and spin very fast. Many stars exist in binary systems with another star, so if this is the case, the neutron star may find itself orbiting another star, and because it is such a compact object, it can steal matter from that star. So the material from the other star approaches the neutron star, but can't quite reach the surface because of the intense pressure of the magnetic field. What happens instead is what you can see in the cover image of this post: the material follows the magnetic field lines to the magnetic poles of the neutron star. 

When this matter hits the surface of the neutron star, it produces light - X-rays to be precise. You can think of it in the same way as a meteor entering the Earth's atmosphere - it's motion creates light (although the exact process is slightly different). This means that we get these two bright spots on the surface of the neutron star, and because it is also rotating very fast, we might see these spots as pulses of light - like a lighthouse coming and going. This is called an X-ray pulsar.

One of the big problems we face is that we still do not know the exact processes that are going on, nor do we even know how much of the light we see comes from which pole (in technical terms, we do not know what the decomposition of the pulse profile is)! This is the problem that I tried to solve in my thesis, using a technique that we all know from parties. 
<img src="/img/science/BSS_horizontal_Copy.png" alt="xConcept of blind source separation. Showing the mixing and subsequent unmixing of two source signals."/>
At a party, we can easily 'tune in' to a conversation, even in the midst of multiple conversations and noise. We can separate the signal quite nicely, even without knowing exactly how the mixing is done. Our brains can do this easily, but it is difficult for a computer. But not impossible. There are several techniques that do this, and one of them is called Non-Negative Matrix Factorisation (NMF).

The overall problem is known as "blind source separation" and I took this NMF method and applied it to my problem and then called it "phase correlated variability analysis". As a test case, I chose one of the brightest X-ray pulsars we know - called Centaurus X-3. I analysed this source and got some interesting and somewhat unexpected results!

And that's it, now we can understand the title [Blind source separation for decomposing X-ray pulsar profiles]. Introducing phase-correlated variability analysis (PCVA) with a case study of Cen X-3](https://www.aanda.org/articles/aa/abs/2024/03/aa47432-23/aa47432-23.html). If you want more information, check out the article itself! And the code for this work is available as a Jupyter notebook on GitHub [here](https://github.com/isaathoff/pcva).