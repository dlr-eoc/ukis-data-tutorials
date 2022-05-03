# [![UKIS](https://raw.githubusercontent.com/dlr-eoc/ukis-pysat/master/docs/ukis-logo.png)](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) UKIS data-tutorials

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dlr-eoc/ukis-data-tutorials/HEAD)
[![GitHub license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

Notebooks and collection of resources around the datasets we published on [Geoservice](https://geoservice.dlr.de/web/).

## burnt area products
Daily, monthly and yearly burnt area products in the EOC Geoservice.

In [burntarea/analyze_data.ipynb](burntarea/analyze_data.ipynb) you can find some small example for how to get and use the products.

The [daily product](https://geoservice.dlr.de/web/maps/eoc:burntarea:efr:daily) is based on a fully automated approach and provides the extents of burned areas two hours after the according scenes have been acquired by the Copernicus Sentinel-3 satellite. Additionally, attribute information about the severity of the fire as well as the exact detection time is included in the data. It is also possible to accurately track the evolution of each burnt area. The product is iteratively and automatically updated over a period of 10 days as new satellite data becomes available. This enables the continuous improvement of the accuracy of the derived extents by minimizing the influence of disturbing factors such as cloud cover. In addition to a daily product, the results are also available in summarized form as [monthly](https://geoservice.dlr.de/web/maps/eoc:burntarea:efr:monthly) and yearly [composites](https://geoservice.dlr.de/web/maps/eoc:burntarea:efr:yearly). While the information of the daily product is always kept for the last 50 days, the archived monthly products are available as early as April 2016, and the first yearly product as early as 2017. This time series allows deriving large-scale developments in terms of size of affected areas and severity. In total, approximately 100,000 satellite scenes from the Ocean and Land Colour Instrument (OLCI) sensor on the Copernicus Sentinel-3 A/B satellites have been used for processing through the end of 2021. Via Web Map and Web Feature Services (WMS/WFS), the data can be easily integrated into existing projects and applications. The methodology for deriving fire areas has been scientifically [published](https://www.mdpi.com/2072-4292/12/13/2162), and an analysis of large fires on the Australian East Coast in 2019/20 based on the methodology is also [available](https://www.mdpi.com/2072-4292/13/24/4975).

[EOC News article](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-18220/29005_read-77114/).

## water products ([Data4Human](https://www.dlr.de/content/en/images/2020/2/data4human-automated-damage-analysis.html) Sentinel-1 Floodmasks)
Sentinel-1 based floodmask products processed within the project Data4Human [available as STAC collection](https://geoservice.dlr.de/eoc/ogc/stac/collections/D4H) on the EOC Geoservice. Checkout [this notebook](water/access_data4human.ipynb) for examples on how to access and interact with the products.

## Licenses
This software is licensed under the [Apache 2.0 License](https://github.com/dlr-eoc/ukis-data-tutorials/blob/main/LICENSE.txt).

Copyright (c) 2022 German Aerospace Center (DLR) * German Remote Sensing Data Center * Department: Geo-Risks and Civil Security

## Contributing
The UKIS team welcomes contributions from the community.
For more detailed information, see our guide on [contributing](https://github.com/dlr-eoc/ukis-data-tutorials/blob/main/CONTRIBUTING.md) if you're interested in getting involved.

## What is UKIS?
The DLR project Environmental and Crisis Information System (the German abbreviation is UKIS, standing for [Umwelt- und Kriseninformationssysteme](https://www.dlr.de/eoc/en/desktopdefault.aspx/tabid-5413/10560_read-21914/) aims at harmonizing the development of information systems at the German Remote Sensing Data Center (DFD) and setting up a framework of modularized and generalized software components.

UKIS is intended to ease and standardize the process of setting up specific information systems and thus bridging the gap from EO product generation and information fusion to the delivery of products and information to end users.

Furthermore, the intention is to save and broaden know-how that was and is invested and earned in the development of information systems and components in several ongoing and future DFD projects.
