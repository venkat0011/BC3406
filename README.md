# BC3406

<!-- ABOUT THE PROJECT -->
## Business analytic consulting Project

In this course, the team collobrated with AON to investigate the impacts of microplastic on aquaculture.
The team gathered microplastic data from NCEI https://www.ncei.noaa.gov/maps/microplastics/ 

![image](https://user-images.githubusercontent.com/76080326/200113906-1b8c91e9-38ea-4819-8aa6-319c802762e1.png)

and aquaculture production data from https://www.fao.org/fishery/en/collection/global_production

![image](https://user-images.githubusercontent.com/76080326/200113896-ad599ba4-dae9-4807-8511-a39169edab96.png)


Both of these datasets do not have any similar primary key except the location. So the concentration of microplastic was mapped into one of the fishing area blocks using QGIS( Similar to ArcGis). We grouped the orange dots ( microplastic) into one of the grids ( fishing area)
![image](https://user-images.githubusercontent.com/76080326/200113952-90dea3b9-b738-49c5-88bb-c252aebfa8db.png)


The team also investigated how the distance of these microplastic affects to the fisheries affect the aquaculture production. The location of the fishrey resources were obtained from https://www.fao.org/figis/geoserver/firms/ows?SERVICE=WFS&request=GetFeature&version=1.0.0&typeName=fishery_all_points&outputFormat=SHAPE-ZIP&format_options=filename:firms-fishery_all_points.zip

The red dots represent microplastic, the brown areas area the fishing areas and the black dots represent the fisheries. The distance is calculated using the existing functions in Qgis
![image](https://user-images.githubusercontent.com/76080326/200114039-c2e629ec-535f-458f-bdd0-05cc94430002.png)




The explroation of the data is in the PowerBi dashboard  https://github.com/venkat0011/BC3406/blob/main/project%20analysis.pbix

The team developed a panel regression model to identify the trends of across the different species of aquaculture and found that some species are positvely correlated with the amount of microplastic and the others are negatively correlated. Since the positive correlation doesn't make sense the team createad a CART model to explain these differences and it was found that those species that were positvely correlated had either very  little microplastic or these microplastic are located further away from the fisheries 
