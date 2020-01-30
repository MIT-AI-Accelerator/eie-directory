Earth Intelligence Engine: Info Directory
=========================================
.. figure:: images/fakes000403.png
   :alt: DeepFakes

StyleGan2 Images


.. contents::

Data
---------

Storm EVent ImagRy (SEVIR) 
~~~~~~~~~~~~~~~~~~~~~~~~~~
Over 10k spatially and temporally aligned image sequences from 5 weather sensors, including visible and infrared satellite, weather radar, and the geostationary lightning mapper.  Many samples in SEVIR correspond to NOAA’s Storm Event Database. For more info see [webpage](sevir.mit.edu).  

**Size:** Approximately 1TB.  Total number of videos: 76k   Total number of image frames across all videos:   3.7 million 

**Location:** Available on MIT Supercloud system (requires you to be a member of the EarthIntelligence group).  Located in EarthIntelligence/datasets/SEVIR 

**Link:**  Not yet available.   We plan to upload to AWS in summer 2020. 

**Other info:** Dataset tools located in [repository](https://github.com/MIT-AI-Accelerator/eie-sevir).

 

Satellite images 
~~~~~~~~~~~~~~~~
Images of Earth ranging from 250m resolution to 3m resolution and with frequency bands ranging from RGB-IR to 36 bands. 

**Size:** many Terabytes.  

**Location:** AWS, NASA, Planet, and other locations 

**Link:** [worldview](https://worldview.earthdata.nasa.gov/)

 

Chesapeake Conservancy LU/LC data 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
High-res aerial imagery from the USDA NAIP program, high-res land cover labels, low-res land cover labels from the USGS NLCD 2011 dataset, low-res multi-spectral imagery from Landsat 8, and high-res building footprint masks from Microsoft Bing, formatted to accelerate machine learning research into land cover mapping. 

**Size:** Nearly 1 TB. 

**Link:** [Dataset Homepage](http://lila.science/datasets/chesapeakelandcover)

Models
---------

StyleGan2 
~~~~~~~~~
**Inputs:** Image Data 
**Outputs:** Image Data 
**Description:** GAN for generating synthetic images from input data distribution, can be used to mix "styles", e.g. winter to summer. 
**Location:**  several branches have been made to support running on supercloud, satori, and local clusters. Weights coming soon. 
**Link(s):** [EIE Forked Repository](https://github.com/MIT-AI-Accelerator/stylegan2)
[general utils for satellite data](https://github.com/MIT-AI-Accelerator/eie-utils)
 

Satellite segmentation model 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
**Inputs:** 1-m resolution satellite imagery. 
**Outputs:** 5-class segmentation map.  
**Description:** U-Net deep architecture. 
**Link:** https://github.com/calebrob6/land-cover 

 
Infrastructure
--------------
MIT Supercloud 
~~~~~~~~~~~~~~
**Purpose:** Large scale computing,  large disk storage,  GPU access. 
**Description:** The SuperCloud allows for large batch processing that can be done in parallel, and access to dual v100 gpu nodes 
**Link:** supercloud.mit.edu 


Satori cluster 
~~~~~~~~~~~~~~
**Purpose:** Large scale gpu computing, large ram and nvlink/infiniband support 
**Description:** The satori cluster allows for large scale gpu batch processing. 
**Link:** https://github.com/mit-satori/  

-  Still need help ? Email petermor@mit.edu
