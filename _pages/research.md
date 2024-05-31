---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---


{% include base_path %}

Covariance Dynamics in Data Assimilation 
======
Uncertainty quantification, particularly the covariance, is crucial for numerical weather prediction (NWP) models, and there are still parts of how the covariance evolves in time that we don’t fully understand. My research looks at this covariance propagation, studying the mathematical equations that describe its time evolution and how we solve these equations during data assimilation. By taking a fundamental look at these equations, I am seeking a better understanding of behaviors observed in current NWP models, such as variance loss, to improve our ability to more accurately forecast weather and provide better preparedness for severe weather events. This research involves different areas of mathematics: statistics, functional analysis, partial differential equations, and numerical analysis.

![image](/images/cndiags_cLto0_gc.png "Examples of inaccurate variance propagation")
The above figure is an example of how standard, full-rank covariance propagation using a Crank-Nicoloson finite difference scheme can produce covariance matrix diagonals (color) that are smooth, but wholly inaccurate. We observe not only variance loss, but also variance gain, both of which can cause problems during data assimilation. See [Gilpin et. al., (2022)](https://doi.org/10.1137/21M1442449) for more details.

Relevant Publications
------
Gilpin, S., Matsuo, T., and Cohn, S.E., 2022: Continuum covariance propagation for understanding variance loss in advective systems, SIAM/ASA J. Uncertainty Quantification, 10, 886 – 914, [https://doi.org/10.1137/21M1442449](https://doi.org/10.1137/21M1442449).

Covariance Modeling
======
Covariance modeling is a challenging and highly relevant problem in both spatial statistics and data assimilation applications. Often, parametric correlation functions are used to construct correlation fields from a finite number of parameters to then model covariances. The figure below is an example of the Generalized Gaspari-Cohn correlation matrix from [Gilpin et al., (2023)](https://doi.org/10.1002/qj.4490), which generalizes the Gaspari-Cohn correlation function commonly used in data assimilation applications. The Generalized Gaspari-Cohn correlation function can generate correlations that are highly anisotropic and compactly supported on non-uniform domains, making it a powerful tool for covariance modeling.

![image](/images/Gilpin_fig5.png "Example of Generalized Gaspari-Cohn on the Unit Circle")

Relevant Publications
------
Gilpin, S., Matsuo, T., and Cohn, S.E., 2023: A generalized, compactly-supported correlation function for data assimilation applications, Q. J. Roy. Meteor. Soc., 149, 1953 - 1989, [https://doi.org/10.1002/qj.4490](https://doi.org/10.1002/qj.4490).

Gilpin, S., 2023: A generalized Gaspari-Cohn correlation function, (v1.0), Zenodo, [https://doi.org/10.5281/zenodo.7859258](https://doi.org/10.5281/zenodo.7859258).


Radio Occultation
======
Radio occultation (RO) is a method of remote-sensing used to observe Earth's atmosphere. As radiowaves emitted from GPS satellites traverse quasi-horiztontally through our atmosphere, they bend (refract) depending on the atmospheric state. Low-Earth orbiting (LEO) satellites then receive these radiowave signals, which can ultimately produce vertical profiles of lower atmospheric and ionospheric quantities. RO observations are assimilated into numerical weather prediction models and have been shown to make a significant impact.

While working for the Constellation Observing System for Meteorology, Ionosphere and Climate ([COSMIC](https://www.cosmic.ucar.edu)) Program at UCAR, I worked on small projects with the aim of improving co-locations methods for RO-radiosonde comparisons and investiagating the errors introduced during vertical interpolation of refractivity during RO data assimilation.

![image](/images/rors_elipse_example.png)
Traditional co-location methods used for comparing atmospheric observations are circles: observations are compared within a fixed distance of a specified location. In [Gilpin et. al., (2018)](https://doi.org/10.5194/amt-11-1-2018), we propose to co-locate observations using elipses oriented along the direction of the wind, rather than circles, to reduce representativeness errors during RO-radiosonde comparisions. 

Relevant Publications
------
Gilpin, S., Rieckh, T., and Anthes, R., 2018: Reducing representativeness errors during radio occultation – radiosonde comparisons, Atmos. Meas. Tech., 11, 269-289, [https://doi.org/10.5194/amt-11-1-2018](https://doi.org/10.5194/amt-11-1-2018).


Gilpin, S., Anthes, R., and Sokolovskiy, S., 2019: Sensitivity of forward-modeled bending angles to vertical interpolation of refractivity for radio occultation data assimilation, Mon. Wea. Rev., 147, 2567–2582, [https://doi.org/10.1175/MWR-D-18-0223.1](https://doi.org/10.1175/MWR-D-18-0223.1)
