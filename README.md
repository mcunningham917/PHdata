# PHdata

`PHdata` provides all digital elevation model data GeoTIFF files used to create 
[Cunningham et al. (2019)](https://mcunningham917.github.io/PHdoc/Publications).
The data are [ten 1-arcsecond (projected at 30m resolution) Shuttle Radar Topography Mission (SRTM) DEMs of tropical mountain](https://mcunningham917.github.io/PHdoc/Data/). 
Voids in 1-arcsecond data are patched with void-filled 3-arcsecond SRTM digital topography
 (projected at 90m resolution and resampled to 30m resolution, acquired from 
 [ViewFinderPanoramas](http://www.viewfinderpanoramas.org/Coverage%20map%20viewfinderpanoramas_org3.htm)).
  An example of one mountain range DEM is provided for 
  [Costa Rica](https://github.com/mcunningham917/PHdata/tree/master/CostaRica/DEM). 

Each mountain range was segmented into large catchments, termed "supercatchments", 
which are fed directly in the 
[Progressive Hypsometry routine](https://mcunningham917.github.io/PHdoc/Method/). 
The catchments extend from a low elevation (usually between 150-250m ASL) and span 
to the main divide of each ROI mountain range. 

## Data organization

The data are organized such that they can be read directly in the `PHtools` algorithm, in 
[PHtools](https://github.com/mcunningham917/PHtools).  
Each ROI has a folder that contains all supercatchments used for the analysis. All results of
the PH analysis are stored in [PHanalysis](https://github.com/mcunningham917/PHanalysis). In `PHanalysis`,
a script for each ROI (e.g.,[`CostaRica.m`](https://github.com/mcunningham917/PHanalysis/blob/master/CostaRica.m)) 
can be used to recreate the output in its entirety.
