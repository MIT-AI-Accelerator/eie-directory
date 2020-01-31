Earth Intelligence Engine: Info Directory
=========================================

.. contents::

Data
---------

Storm EVent ImagRy (SEVIR) 
~~~~~~~~~~~~~~~~~~~~~~~~~~
.. figure:: images/sevir_frames.png
   :alt: Sevir Data Generator
Over 10k spatially and temporally aligned image sequences from 5 weather sensors, including visible and infrared satellite, weather radar, and the geostationary lightning mapper.  Many samples in SEVIR correspond to NOAA’s Storm Event Database. For more info see (sevir.mit.edu).  

**Size:** Approximately 1TB.  Total number of videos: 76k   Total number of image frames across all videos:   3.7 million 

**Location:** Available on MIT Supercloud system (requires you to be a member of the EarthIntelligence group).  Located in EarthIntelligence/datasets/SEVIR 

**Link:**  Not yet available.   We plan to upload to AWS in summer 2020. 

**Other info:** Dataset tools located in sevir_.

 

Satellite images 
~~~~~~~~~~~~~~~~
.. figure:: images/worldview.jpg
   :alt: Tropical Cyclone Idai
Images of Earth ranging from 250m resolution to 3m resolution and with frequency bands ranging from RGB-IR to 36 bands. 

**Size:** many Terabytes.  

**Location:** AWS, NASA, Planet, and other locations 

**Link:** worldview_

 

Chesapeake Conservancy LU/LC data 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
High-res aerial imagery from the USDA NAIP program, high-res land cover labels, low-res land cover labels from the USGS NLCD 2011 dataset, low-res multi-spectral imagery from Landsat 8, and high-res building footprint masks from Microsoft Bing, formatted to accelerate machine learning research into land cover mapping. 

**Size:** Nearly 1 TB. 

**Link:** landcover_data_

Models
---------

StyleGan2 
~~~~~~~~~
.. figure:: images/fakes000403.png
   :alt: DeepFakes
**Inputs:** Image Data 

**Outputs:** Image Data 

**Description:** GAN for generating synthetic images from input data distribution, can be used to mix "styles", e.g. winter to summer. 

**Location:**  several branches have been made to support running on supercloud, satori, and local clusters. Weights coming soon. 

**Link(s):** stylegan2_ , imagery_utils_
 

Satellite segmentation model 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
**Inputs:** 1-m resolution satellite imagery. 

**Outputs:** 5-class segmentation map.  

**Description:** U-Net architecture. 

**Link:** landcover_model_

 
Infrastructure
--------------
MIT Supercloud 
~~~~~~~~~~~~~~
**Purpose:** Large scale computing,  large disk storage,  GPU access. 

**Description:** The SuperCloud allows for large batch processing that can be done in parallel, and access to dual v100 gpu nodes 

**Link:** supercloud_


MIT Satori  
~~~~~~~~~~~~~~
**Purpose:** Large scale gpu computing, large ram and nvlink/infiniband support 

**Description:** The satori cluster allows for large scale gpu batch processing. 

**Link:** satori_

-  Still need help ? Email petermor@mit.edu
.. _satori: https://github.com/mit-satori/
.. _supercloud: https://supercloud.mit.edu
.. _landcover_model: https://github.com/calebrob6/land-cover
.. _stylegan2: https://github.com/MIT-AI-Accelerator/stylegan2
.. _imagery_utils: https://github.com/MIT-AI-Accelerator/eie-utils
.. _landcover_data: http://lila.science/datasets/chesapeakelandcover
.. _worldview: https://worldview.earthdata.nasa.gov/
.. _sevir: https://github.com/MIT-AI-Accelerator/eie-sevir
