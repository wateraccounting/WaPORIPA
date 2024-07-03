# <font color='#ff009a'> WaPORIPA(beta): Standardized protocol for irrigation performance assessment using WaPOR data. </font>
![img](https://github.com/wateraccounting/WaPORIPA/blob/main/images/Image2.png) 

**Authors:** 
* Abebe D. Chukalla (a.chukalla@un-ihe.org),
* Suzan Dehati,
* Solomon Seyoum,
* Bich Tran,
* Marloes Mul
  
  
© IHE Delft Institute for Water Education, June 2024

Note: The script is also used in on-campus short course on ['Remote Sensing for Agricultural Water Management'](https://www.un-ihe.org/courses/on-campus/remote-sensing-agricultural-water-management) organised annually by IHE Delft Institute for Water Education. Next edition: 3-14 March 2025. 

![img](https://github.com/wateraccounting/WaPORIPA/blob/main/images/Short%20course%20RS4AWM.png)
#
The objective of this repository is to calculate irrigation performance indicators using WaPOR data. It can accomodate two options for the water use and production data, the WaPOR version 3 data (downloaded using [Download_WaPORv3_data script](https://github.com/wateraccounting/WaPORMOOC/tree/main/1_WaPOR_download_colab) or data created using [pyWaPOR](https://bitbucket.org/cioapps/pywapor/src/master/). The scripts are updated from [WaPORWP](https://github.com/wateraccounting/WAPORWP) to allow for the use of WaPOR version 3 and pyWaPOR outputs. The current repository is a beta version which contains 4 modules:

- Module 1a: Seasonal aggregation of WaPORv3 AETI, T and NPP
- Module 1b: Seasonal aggregation of pyWaPOR outputs AETI, T and NPP (script also allows for exporting dekadal and monthly timeseries)
- pre-Module 2: Clipping seasonal data to Area of Interest (AOI) (optional, but important for interpretation of IPA)
- Module 2: Calculate yield, water productivity and irrigation performance indicators
  
![img](https://github.com/wateraccounting/WaPORIPA/blob/main/images/WaPORIPA_beta.jpg)

## Irrigation performance indicators 
The following performance indicators are included in the repository (see for more information [Chukalla et al., 2022](https://hess.copernicus.org/articles/26/2759/2022/hess-26-2759-2022.html))

Land and water productivity
- Water consumption (AETI)
- Dry biomass production and yield (requires crop type information)
- Water Productivity (biomass and/or crop)

Irrigation performance indicators
- Adequacy compared to 95th percentile
- Beneficial Fraction
- Uniformity
- Relative water deficit

To be able to interpret the analyses, it is important to have crop type information for the AOI. See [WaPORMOOC repository](https://github.com/wateraccounting/WaPORMOOC/tree/main) for examples on how to do zonal statistics using crop type information. 

We are working on developing more analyses which will be made available in a WaPORIPA version 1. This will include adding more calculations, such as blue ET, crop water requirement (CWR) and adequacy compared to CWR. In addition, we will update the crop and yield gap script from [WaPORWP](https://github.com/wateraccounting/WAPORWP). 

## Requirements
All scripts can be run in Colab or on a local computer (see for example of [installation instructions for mamba](https://courses.gisopencourseware.org/mod/book/view.php?id=430&chapterid=1427) with lots of interesting educational materials. For a good understanding of the scripts presented here, we advise to have followed (and completed our open access course on ['Python for Geospatial analyses using WaPOR data'](https://ocw.un-ihe.org/user/index.php?id=272))
![image](https://github.com/wateraccounting/WaPORMOOC/blob/main/images/Banner%2Cpython%2CWaPOR.jpeg)

## Acknowledgements
This repository was developed as part of the [“Monitoring land and water productivity by Remote Sensing (WaPOR phase 2) project”](https://www.fao.org/in-action/remote-sensing-for-water-productivity/en/) led by FAO and funded by the Ministry of Foreign Affairs of the Netherlands. 
