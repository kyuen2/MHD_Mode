# MHD_Mode

Ka Ho Yuen @ UW Madison, last updated Apr 25, 2022.

**TL;DR**: The main Code used in Yuen et.al (2022, codename "leakage"), Lazarian, Yuen, Pogosyan (2022ab, codename "DMA,MM2"). 

Credits: Equations are rendered via  https://www.codecogs.com/latex/eqneditor.php 

## What is this repository about?

The estimation of magentic field strength properties relies the detailed knowledge of MHD modes. However, there are not much information aside from reading papers. This repository aims at providing the minimal information for you to kickstart with the analysis of B-field strengths in MHD turbulence.

## So what is the current state of magnetic field strength estimation in interstellar media as of now (Apr 2022)?

The Davis (1951)- Chandrasekhar-Fermi (1953) method is one of the most important method in estimating the magnetic field strength in interstellar media (ISM). In short, considering _ideal Alfven-wave turbulence with energy partition between kinetic and magnetic field_ we can correlate the _first order fluctuations of velocity and magnetic field fluctuations of Alfven wave_ via the following formula

<img src="https://latex.codecogs.com/svg.image?\frac{1}{2}\rho&space;\delta&space;v^2&space;=&space;\frac{\delta&space;B^2}{8\pi}" title="https://latex.codecogs.com/svg.image?\frac{1}{2}\rho \delta v^2 = \frac{\delta B^2}{8\pi}" />

which leads to a handy formula for magnetic field strength estimation which now the astrophysical community called it the **DCF technique**:

![equation](https://latex.codecogs.com/svg.image?B=\sqrt{4\pi\rho}\frac{\delta&space;v}{\delta&space;\phi})

where  <img src="https://latex.codecogs.com/svg.image?\delta&space;\phi&space;=&space;\delta&space;B/B" />. In observations, <img src="https://latex.codecogs.com/svg.image?\delta&space;v" title="https://latex.codecogs.com/svg.image?\delta v" /> is the **Line-of-sight velocity dispersion** and <img src="https://latex.codecogs.com/svg.image?\delta&space;\phi" title="https://latex.codecogs.com/svg.image?\delta \phi" /> is the **Plane-of-sky _polarization_ angle dispersion**.

The community has realized a few decades ago that this formula is not that accurate. Earlier people inserts a f_0 term :

<img src="https://latex.codecogs.com/svg.image?B={\color{DarkOrange}&space;f_0}&space;\sqrt{4\pi\rho}\frac{\delta&space;v_{LOS}}{\delta&space;\phi_{POS}}" title="https://latex.codecogs.com/svg.image?B={\color{DarkOrange} f_0} \sqrt{4\pi\rho}\frac{\delta v_{LOS}}{\delta \phi_{POS}}" />

which this f_0 term is traditionally assumed to be a constant of value 0.5-2. Unfortunately, the community identifies more problems recently, the following list is not exhaustive:
- **Cho & Yoo 2016**: The f_0 constant is a function of number of independent turbulent eddies along the line of sight. In short, they replace <img src="https://latex.codecogs.com/svg.image?\delta&space;v" title="https://latex.codecogs.com/svg.image?\delta v" /> to <img src="https://latex.codecogs.com/svg.image?\delta&space;C&space;" title="https://latex.codecogs.com/svg.image?\delta C " />, the dispersion of velociy centroid.
- **Skaliais & Tassis 2021, Skaliais et.al 2021**: The form of the DCF equation is suggested to be wrong when compressibility comes into play. In short they suggest an alternative formula <img src="https://latex.codecogs.com/svg.image?B=\sqrt{2\pi\rho}\frac{\delta&space;v_{LOS}}{\sqrt{\delta&space;\phi_{POS}}" title="https://latex.codecogs.com/svg.image?B=\sqrt{2\pi\rho}\frac{\delta v_{LOS}}{\sqrt{\delta \phi_{POS}}" />
- **Lazarian, Yuen, Pogosyan 2022a (arXiv: 2204.09731, ApJ in production)**: f_0 depends on a lot of things, including the Alfvenic Mach number, the line of sight angle (the angle between magnetic field and line of sight), and the fraction of modes.

## So how to start with?

My suggestion to the readers is to go to the templates that I included in this repository. 



