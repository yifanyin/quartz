---
title: 2024 Hualien earthquake
date: 2024-04-25
tags:
  - earthquake
aliases:
  - 2024 Hualien earthquake
---
# Metadata
- Magnitude:
	- CWA Taiwan: $M_L$ 7.2
	- USGS: $M_W$ 7.4
# Resource
- [USGS finite fault solution](https://earthquake.usgs.gov/earthquakes/eventpage/us7000m9g4/finite-fault) shows that the earthquake rupture and expand unidirectionally to the north. The fault plane dips to the east. The solution fit the aftershock distribution, too.
- Taiwan Earthquake Research Center's [rapid report](https://tec.earth.sinica.edu.tw/specialEQ/pdf/20240403hwalien.pdf) in Chinese.

# Exploratory analysis
Below are some plots I produced in preparation for a radio interview. The catalogs comes from the [Seismological Center of the Central Weather Agency, Taiwan](https://scweb.cwa.gov.tw/en-us/earthquake/data).

First up is the magnitude versus time plot. The rate decrease with time, however even at 14 days after, there is still magnitude-five event.
![[mag-time.png]]
Next up, I use the proposed aftershock decay relation from [Page et. al. (2016)](https://doi.org/10.1785/0120160073). The relation also help gauging the aftershock rate into the future.
![[aftershock-decay.png]]

Then I look at the space-time distribution of the aftershocks. I have no idea how accurate the initial catalog is. This provide a rough estimate of the fault plane.
![[aftershocks-3d.png]]