---
priority: 0.6
title: Grid-tied with backup Photovoltaic system
excerpt: in collaboration with Sunteq
categories: works
background-image: ESS/solar.jpg
tags:
  - Photovoltaic
  - ESS
  - Welding
  - HomeAssistant
---


I always dreamd about a grid-tied photovoltaic system with backup capability. However most grid-tied installations ([98%](https://www.solaireoccitanie.fr/details-installation+solaire+en+autoconsommation+autonome+en+cas+de+coupure+de+reseau+a+toulouse-91)) must shut down during a grid failure to comply with anti-islanding protection (IEC 62116 / EN 50549-1). 

My system features the Victron MultiPlus-II, which incorporates a two-point disconnection relay that ensures complete electrical isolation from the grid during outages, allowing it to safely operate in island mode and continue powering the house from photovoltaic/batteries without any risk of backfeeding into the grid.

## Solar panels

{% capture solar_content %}

6kWp photovoltaic installation done by [Sunteq](https://sunteq.fr/) company, which I highly recommend!
{% endcapture %}

{% include pic_with_content.html pos="right" src="/images/ESS/solar.jpg" content=solar_content %}

## ESS installation

{% capture ess_content %}
Here is the architecture I designed and installed. It was fully-verified, end-connected and validated by [Sunteq](https://sunteq.fr/):

- VICTRON SmartSolar MPPT RS 450/100-MC4 (using 2 MPPT lines of 3kWp each)
- VICTRON MultiPlus-II GX 48/5000/70-50 230V (I'm not using the GX part in the end)
- VICTRON - Cerbo GX MK2 
- VICTRON - Lynx Distributor
- Pylontech Lithium 4.8kWh - US5000 48V 100A

Don't forget to have a look (top right corner) at the 40Kg battery stored in the welded rack described below.

{% endcapture %}

{% include pic_with_content.html pos="left" src="/images/ESS/elec_full.jpg" content=ess_content %}

## Battery rack welding

{% capture cutting_content %}
Cutting the side panels
{% endcapture %}

{% include pic_with_content.html pos="right" src="/images/ESS/cutting.jpg" content=cutting_content %}

{% capture rack_content %}
Raw rack I welded with flux-cored wire
{% endcapture %}

{% include pic_with_content.html pos="left" src="/images/ESS/rack_raw.jpg" content=rack_content %}


{% capture painted_content %}
And a coat of spray paint!
{% endcapture %}

{% include pic_with_content.html pos="right" src="/images/ESS/painted.jpg" content=painted_content %}

## Home Assistant integration

{% capture ha_content %}
All the home's energy is managed on my local Home Assistant server where my own EMS (Energy Management System) runs
{% endcapture %}

{% include pic_with_content.html pos="left" src="/images/ESS/HA.png" content=ha_content %}