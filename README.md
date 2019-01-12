# PHdata

`PHdata` provides all digital elevation model data GeoTIFF files used to create 
[Cunningham et al. (2019)](https://mcunningham917.github.io/PHdoc/Publications).
The data are ten 1-arcsecond (projected at 30m resolution) 
Shuttle Radar Topography Mission (SRTM) 
[DEMs](https://mcunningham917.github.io/PHdoc/Data/) of tropical mountain ranges. 
Each mountain range was segmented into large catchments, termed "supercatchments", 
which are fed directly in the 
[Progressive Hypsometry routine](https://mcunningham917.github.io/PHdoc/Method/). 
The catchments extend from a low elevation (usually between 150-250m ASL) and span 
to the main divide of each ROI mountain range. 

## Data organization

The data are organized such that they can be read directly in the `PHtools` algorithm, in 
[PHtools](https://github.com/mcunningham917/PHtools).  
Each ROI has a folder that contains all supercatchments used for the analysis. 
[PHanalysis](https://github.com/mcunningham917/PHanalysis) contains a script for each ROI 
(e.g.,
[`CostaRica.m`](https://github.com/mcunningham917/PHanalysis/blob/master/CostaRica.m) 
that accesses the appropriate list of supercatchments and writes 
to its respective folder in `PHanalysis` (for the same example: 
[here](https://github.com/mcunningham917/PHanalysis/tree/master/CostaRica)). 
