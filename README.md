# Project Template
​
## Project Description
​
As the climate changes, the world’s coastlines change through erosion or accretion. In Hawai’i in particular, rising sea levels from climate change cause beach erosion to clash with the state's coastal communities. Observing and modeling how the beaches are changing is an important task for Hawai‘i’s future way of life, but traditional surveying is time and energy consuming over Hawaii’s more than 900 miles of coastline. 
​
Our project, CSTSI (**Coastal Surveillance Through Satellite Imagery**) aims to automatically and accurately detect past shoreline positions of Hawaii's coastlines to inform shoreline evolution models using the power of satellite imagery. CSTSI sources a myriad of satellite sources with different temporal and spatial resolutions – including Landsat, Sentinel, and PlanetScope (Planet Labs). Our project is currently two-fold: 
1) We use the popular open source package CoastSat (Vos, UNSW) for Landsat and Sentinel image sources, while 2) creating a separate but similar framework for Planetscope images, called CoastVision. These two methodologies rely on machine learning for pixel classification through a convolutional neural network, and obtain a shoreline position (water and sand interface) at subpixel resolution by using marching squares or gaussian smoothing. Both frameworks have the ability to do an interactive quality control to accept or discard each shoreline contour, or automatically remove contours that deviate from a set threshold of change or position. The remaining shoreline contours are then fed to outside models such as the CoSMoS-COAST shoreline evolution model, which relies heavily on data assimilation of satellite-derived shorelines to accurately predict future shoreline positions. 
​
CSTSI will be a powerful and comprehensive tool for monitoring shoreline change. It will allow for many projects within our interdisciplinary research group, the Climate Resilience Collaborative (within University of Hawai’i Mānoa) to have reliable and accessible data. The aim is for these data to be implemented into local policy, cited for scientific research, and used by communities and stakeholders for guidance on potential sea level rise hazard zones. Modeled outcomes will be presented on public webmaps, as used case-studies for specific high-risk areas on Hawai‘i. 
​
## Objectives
​
The objective is to effectively and automatically map shoreline positions for all of Hawai‘i's beaches since 1990, to inform modelling of shoreline change and projections into the future. We are using satellite images from Landsat (~1990-present), Sentinel (~2015-present), and PlanetScope (~2017-present). For each image, we are currently outputting 
1) pixel classification (.tiff)
2) shoreline contour (.geojson)
3) beach width at cross shore transects located every 20m along the coast (.csv - row:datetime, column:transectID)
With Azure, we aim to move some of these processes (obtaining and temporarily storing data; processing the pixel classification and transect intersections) onto the cloud to increase datasharing, computing efficiency, and collaboration
​
## Deliverables
​
- A comprehensive database of satellite and airborne imagery of Hawaii’s beaches (using Azure DataShare)
- Scientific publications and reports on the CSTSI framework, results of CoSMoS-COAST Hawaii and of CSTSI.
- Open source code of CoastVision package and workflow available on GitHub for other researchers to use for shoreline extraction research on PlanetScope Imagery
- Multi-Year end goal: Sea Level Rise web map viewer with data available for future coastal hazard zones and shoreline positions every 20m of Hawai‘i’s shoreline. This, in conjunction with other products produced by CRC, will provide the foundation of our SLR, erosion, and coastal hazard viewer 2.0 - an update and extension of the PacIOOS viewer: https://www.pacioos.hawaii.edu/shoreline/slr-hawaii/ 
​

## Contributors

Anna Mikkelsen / Climate Resilience Collab - UH Mānoa / abmikkelsen / abm20@hawaii.edu
Richelle Moskvichev / Climate Resilience Collab - UH Mānoa/ rcabatic / rum@hawaii.edu 
Erica Ta / Climate Resilience Collab - UH Mānoa/ taerica / ericata@hawaii.edu
Joel Nicolow / Climate Resilience Collab - UH Mānoa / jcnicolowUH / jnicolow@hawaii.edu

------
With the Climate Resilience Collaborative (CRC) - University of Hawai‘i at Mānoa
------
