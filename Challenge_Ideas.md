## Earthday Hackathon

#### Data
* SEVIR ( 5 sensor inputs easy for ml format )
* Numerical Weather Model Output + Potentially with overlapping data sources
* Synthetic Ocean Model Proxies + Potentially scrap data sources
* Satellite imagery (planet data, landsat, modis, sentinel, chespeake, hyperspectral)

#### Hackathon Tracks & Challenge Ideas
* Interpretability and Visualization
How can I intuitively represent predictive data for climate and weather? 

* Representation and transfer learning
How can use other datasets or self supervision tasks to learn features which can be broadly applied to other climate and weather problems
  * Challenge 1 idea : Provide a feature embedding that can be fine tuned on a hidden task and evaluated

* Robustness and Physical Constraints
  * Challenge 1 idea : Perform a task well even with noise
  * Challenge 2 idea : Enforce that a predictive model follows physical constraints of a system
  * Challenge 3 idea : Break a model for nwp or classification under some input pertubation constraint
  * Challenge 4 idea : anomaly detection in input 

* Unsupervised learning and Data Imputation
How can we develop algorithms which can be indirectly evaluated 
  * Challenge 1 idea : estimate flow field from satellite images and synthetic imagery 
  * Challenge 2 idea : Sensor fusion or prediction (given 4 sensors predict 5)





