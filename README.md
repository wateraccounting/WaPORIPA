# <font color='#ff009a'> WaPORIPA: Standardized protocol for irrigation performance assessment using WaPOR data. </font>

**Authors:** 
* Abebe D. Chukalla (a.chukalla@un-ihe.org),
* Suzan Dehati,
* Solomon Seyoum,
* Bich Tran,
* Marloes Mul
   
(c) IHE Delft, June 2024

Note: The script is also used in on-campus short course on ['Remote Sensing for Agricultural Water Management'](https://www.un-ihe.org/courses/on-campus/remote-sensing-agricultural-water-management) organised annually by IHE Delft Institute for Water Education. Next edition: March 2025. 

The objective of this repository is to calculate irrigation performance indicators using WaPOR data. It can accomodate two options for the water use and production data, the WaPOR version 3 data (downloaded using [Download_WaPORv3_data script](https://github.com/wateraccounting/WaPORMOOC/tree/main/1_WaPOR_download_colab) or data created using [pyWaPOR](https://bitbucket.org/cioapps/pywapor/src/master/). The scripts are updated from [WaPORWP](https://github.com/wateraccounting/WAPORWP) to allow for the use of WaPOR version 3 and pyWaPOR outputs. This repository consists of 5 modules:

- Module 1: Calculate seasonal maps and resample WaPOR climate data (RET & PCP)
- Module 2a: Seasonal aggregation of WaPORv3 AETI, T and NPP
- Module 2b: Seasonal aggregation of pyWaPOR outputs AETI, T and NPP (script also allows for exporting dekadal and monthly timeseries)
- pre-Module 3: Clipping seasonal data to Area of Interest (AOI) (optional)
- Module 3: Calculate yield, water consumption and irrigation performance indicators
  
![image](https://github.com/wateraccounting/WaPORIPA/blob/main/images/WaPORIPA%20%E2%80%93%20github%20repo%20structure.jpg)

## Irrigation performance indicators 
The following performance indicators are included in the repository (see for more information [Chukalla et al 2022](https://hess.copernicus.org/articles/26/2759/2022/hess-26-2759-2022.html))
- Water consumption (AETI)
- Dry biomass production and yield (requires crop type information)
- Water Productivity (biomass and/or crop)
- Adequacy compared to 95th percentile
- Beneficial Fraction
- Uniformity
- Relative water deficit

Over the coming period we will add more calculations, such as blue ET, crop water requirement (CWR) and adequacy compared to CWR. In addition, we will update the crop and yield gap script from WaPORWP. 

## Requirements
All scripts can be run in Colab or on a local computer (see for example of installation instructions of [mamba](https://courses.gisopencourseware.org/mod/book/view.php?id=430&chapterid=1427) with lots of interesting educational materials. For a good understanding of the scripts presented here, we advise to have followed (and completed our open access course on ['Python for Geospatial analyses using WaPOR data'](https://ocw.un-ihe.org/user/index.php?id=272))
![image](https://github.com/wateraccounting/WaPORMOOC/blob/main/images/Banner%2Cpython%2CWaPOR.jpeg)

This repository was developed as part of the [“Monitoring land and water productivity by Remote Sensing (WaPOR phase 2) project”](https://www.fao.org/in-action/remote-sensing-for-water-productivity/en/) led by FAO and funded by the Ministry of Foreign Affairs of the Netherlands. 
