# Project Template

## Project Description

As the climate changes, the world’s coastlines change through erosion or accretion. In Hawai’i in particular, rising sea levels from climate change cause beach erosion to clash with the state's coastal communities. Observing and modeling how the beaches are changing is an important task for Hawaii’s future way of life, but traditional surveying is time and energy consuming over Hawaii’s more than 900 miles of coastline. 

Our project, CSTSI (Coastal Surveillance Through Satellite Imagery) aims to automatically and accurately detect past shoreline positions of Hawaii's coastlines to inform shoreline evolution models using the power of satellite imagery. CSTSI sources a myriad of satellite sources with different temporal and spatial resolutions – including Landsat, Sentinel, and PlanetScope (Planet Labs). Our project is currently two-fold: 1) We use the popular open source package CoastSat (Vos, UNSW) for Landsat and Sentinel image sources, while 2) creating a separate but similar framework for Planetscope images, called CoastVision. These two methodologies rely on machine learning for pixel classification through a convolutional neural network, and obtain a shoreline position (water and sand interface) at subpixel resolution by using marching squares or gaussian smoothing. Contours are then subject to quality control and assurance. Both frameworks have the ability to do an interactive quality control to accept or discard each shoreline contour, or automatically remove contours that deviate from a set threshold of change or position. The remaining shoreline contours are then fed to outside models such as the CoSMoS-COAST shoreline evolution model, which relies heavily on data assimilation of satellite-derived shorelines to accurately predict future shoreline positions. 

CSTSI will be a powerful and comprehensive tool for monitoring shoreline change. It will allow for many projects within our interdisciplinary research group, the Climate Resilience Collaborative (within University of Hawai’i Mānoa) to have reliable and accessible data. The aim is for these data to be implemented into local policy, cited for scientific research, and used by communities and stakeholders for guidance on potential sea level rise hazard zones. Modeled outcomes will be presented on public webmaps, as used case-studies for specific high-risk areas on Hawai‘i. 


## Objectives

**!! TODO:** Enter the objectives of your research project here

## Deliverables

**!! TODO:** Enter the deliverables of your research project here

## Contributors

Anna Mikkelsen / Climate Resilience Collab - UH Mānoa / abmikkelsen / abm20@hawaii.edu
Richelle Moskvichev / Climate Resilience Collab - UH Mānoa/ rcabatic / rum@hawaii.edu 
Erica Ta / Climate Resilience Collab - UH Mānoa/ taerica / ericata@hawaii.edu
Joel Nicolow / Climate Resilience Collab - UH Mānoa / jcnicolowUH / jnicolow@hawaii.edu


