# MHD_Mode

Ka Ho Yuen @ UW Madison

TL;DR: The main Code used in Yuen et.al (2022, codename "leakage"), Lazarian, Yuen, Pogosyan (2022ab, codename "DMA,MM2"). 

## What is this repository about?

The estimation of magentic field strength properties relies the detailed knowledge of MHD modes. However, there are not much information aside from reading papers. This repository aims at providing the minimal information for you to kickstart with the analysis of B-field strengths in MHD turbulence.

## So what is the current state of magnetic field strength estimation in interstellar media as of now (Apr 2022)?

The Davis (1951)- Chandrasekhar-Fermi (1953) method is one of the most important method in estimating the magnetic field strength in interstellar media (ISM). In short, considering ideal Alfven-wave turbulence with energy partition between kinetic and magnetic field:

![equation](https://latex.codecogs.com/svg.image?\frac{1}{2}\rho\delta&space;v^2&space;\approx&space;\frac{\delta&space;B^2}{8\pi})

which leads to a handy formula for magnetic field strength estimation:

![equation](https://latex.codecogs.com/svg.image?B=\sqrt{4\pi\rho}\frac{\delta&space;v}{\delta&space;\phi})

where  <img src="https://latex.codecogs.com/svg.image?\delta&space;\phi&space;=&space;\delta&space;B/B" />
