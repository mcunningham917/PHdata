# PHdata

PHdata provides all data used to create Figure 8a/b in Cunningham et al. (2019). The data are ten 1-arcsecond (projected at 30 m resolution) Shuttle Radar Topography Mission (SRTM) [DEMs](https://mcunningham917.github.io/PHdoc/Data/) of tropical mountain ranges. Each mountain range was segmented into large catchments, termed "supercatchments", which are fed directly in the [Progressive Hypsometry routine](https://mcunningham917.github.io/PHdoc/Method/). The catchments extend from a low elevation (usually between 150-250 m ASL) and span to the main divide of each ROI mountain range. 

## Organization

The data are organized such that they can be read directly in the PH algorithm, in [PHtools](https://github.com/mcunningham917/PHtools).  Each  ROI has a folder that contains all supercatchments used for the analysis. [PHanalysis](https://github.com/mcunningham917/PHanalysis) contains a script for each ROI (ex.: [`CostaRica.m`](https://github.com/mcunningham917/PHanalysis/blob/master/CostaRica.m) that retrieves the appropriate list of supercatchments from this repository and writes to its respective folder in PHanalysis (for the same example: [here](https://github.com/mcunningham917/PHanalysis/tree/master/CostaRica)). 
