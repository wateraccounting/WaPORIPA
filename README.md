# <font color='#ff009a'> WaPORIPA: Standardized protocol for irrigation performance assessment using WaPOR data. </font>

**Authors:** 
* Abebe D. Chukalla (a.chukalla@un-ihe.org),
* Marloes Mul, 
* Suzan Dehati,
* Solomon Seyoum,
* Bich Tran

The objective of this repository is to calculate irrigation performance assessment indicators using WaPOR data. It can accomodate two options for the water use and production data, the WaPOR version 3 data (downloaded using [Download_WaPORv3_data script](https://github.com/wateraccounting/WaPORMOOC/tree/main/1_WaPOR_download_colab) or data created using [pyWaPOR](https://bitbucket.org/cioapps/pywapor/src/master/). The scripts are updated from [WaPORWP](https://github.com/wateraccounting/WAPORWP) to allow for the use of WaPOR version 3 and pyWaPOR outputs. This repository consists of 5 modules:
- Module 1: Calculate seasonal maps and resample WaPOR climate data (RET & PCP)
- Module 2a: Seasonal aggregation of WaPORv3 AETI, T and NPP
- Module 2b: Seasonal aggregation of pyWaPOR outputs AETI, T and NPP (script also allows for exporting dekadal and monthly timeseries)
- pre-Module 3: Clipping seasonal data to Area of Interest (AOI) (optional)
- Module 3: Calculate yield, water consumption and irrigation performance assessment indicators
- 
![image](https://github.com/wateraccounting/WaPORIPA/blob/main/images/WaPORIPA%20%E2%80%93%20github%20repo%20structure.jpg)

This repository was developed as part of the [“Monitoring land and water productivity by Remote Sensing (WaPOR phase 2) project”](https://www.fao.org/in-action/remote-sensing-for-water-productivity/en/) led by FAO and funded by the Ministry of Foreign Affairs of the Netherlands. 

The script is also used in on-campus short course on ['Remote Sensing for Agricultural Water Management'](https://www.un-ihe.org/courses/on-campus/remote-sensing-agricultural-water-management) organised annually by IHE Delft Institute for Water Education 
