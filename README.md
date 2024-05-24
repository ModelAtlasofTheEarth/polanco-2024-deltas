# New [M@TE](https://mate.science/)! model: 
 _we have provided a summary of your model as a starting point for the README, feel free to edit_
## Section 1: Summary of your model   

**Model Submitter:**  

Sara Polanco ([0000-0002-1270-4377](https://orcid.org/0000-0002-1270-4377))

**Model Creator(s):**  

- Sara Polanco ([0000-0002-1270-4377](https://orcid.org/0000-0002-1270-4377))  
- Michael Blum ([0000-0003-0263-0084](https://orcid.org/0000-0003-0263-0084))  
- Tristan Salles ([0000-0001-6095-7689](https://orcid.org/0000-0001-6095-7689))  
- Bruce C Frederick   
- Rebecca Farrington ([0000-0002-2594-6965](https://orcid.org/0000-0002-2594-6965))  
- Xuesong Ding ([0000-0003-3693-932X](https://orcid.org/0000-0003-3693-932X))  
- Ben Mather ([0000-0003-3566-1557](https://orcid.org/0000-0003-3566-1557))  
- Claire A. Mallard ([0000-0003-2595-2414](https://orcid.org/0000-0003-2595-2414))  
- Louis-Noel Moresi ([0000-0003-3685-174X](https://orcid.org/0000-0003-3685-174X))  
  
**Model name:**  

`polanco-2024-deltas` 

(this will be the name of the model repository when created) 

**Model long name:**  

_Flexural isostatic response of continental-scale deltas to climatically driven sea level changes_  

**License:**  

[Creative Commons Attribution 4.0 International]( https://creativecommons.org/licenses/by/4.0/legalcode.txt)

**Model Category:**  

- model published in study   
  
**Model Status:**  

- completed   
  
**Associated Publication title:**  

_[Flexural isostatic response of continental-scale deltas to climatically driven sea level changes](http://dx.doi.org/10.5194/esurf-12-301-2024)_ 

**Abstract:**  

Abstract. The interplay between climate-forced sea level change, erosional and depositional processes, and flexural isostasy in deep time on passive margin deltas remains poorly understood. We performed a series of conceptual simulations to investigate flexural isostatic responses to high-frequency fluctuations in water and sediment load associated with climatically driven sea level changes. We model a large drainage basin that discharges to a continental margin and produces a large deltaic depocenter, then prescribe synthetic and climatic-driven sea level curves of different frequencies to assess flexural response. Results show that flexural isostatic responses are bidirectional over 100–1000 kyr timescales and are in sync with the magnitude, frequency, and direction of sea level fluctuations and that isostatic adjustments play an important role in driving along-strike and cross-shelf river mouth migration and sediment accumulation. Our findings demonstrate that climate-forced sea level changes produce a feedback mechanism that results in self-sustaining creation of accommodation into which sediment is deposited and plays a major role in delta morphology and stratigraphic architecture.
                    

**Scientific Keywords:**  

- Flexural isostasy   
- Glacial isostatic adjustment (GIA)   
- Deltaic depocenters   
- Stratigraphic record   
  
**Funder(s):**  
- Australian Research Council   
- Australian–American Fulbright Commission   
- The University of Melbourne   
  
## Section 2: your model code, output data  

** No embargo on model contents requested****Include model code:**   

True 

**Model code notes:**   

The input and boundary conditions for the model are structured as follows:
an input XML file where the initial and boundary conditions are set
a data folder containing the initial surface and the boundary conditions, in this case different sea-level scenarios
a series of IPython Notebooks used to run the experiment and perform some pre or post-processing tasks. 

**Include model output data:**   

True 

**Model output data notes:**   

The model output data is stored in a hdf5 format. You will see a h5 folder and a series of xdmf files. 
- **h5** folder contains the **hdf5** data, all the information computed by the model are stored in these files. You will have at least the *tin* (surface) and *flow* (stream network) dataset and also the *sed* (stratigraphy) data if the stratal structure is computed in your simulation.

- two **.xdmf** files for the surface (**tin_series.xdmf**) and the flow network (**flow_series.xdmf**) that read the **xmf** files through time. 

## Section 3: software framework and compute details   
**Software Framework DOI/URL:**  

Found software: _[Badlands](https://doi.org/10.5281/zenodo.1069573)_ 

**Software Repository:**   

https://github.com/badlands-model/badlands 

**Name of primary software framework:**  

Badlands 

## Section 4: web material (for mate.science)   
**Landing page image:**  

Filename: [fig1.png](https://github.com/ModelAtlasofTheEarth/model_submission/assets/29790931/166800c8-c053-4a04-a2ae-8526940e6f7b)  
Caption: Our simulations produce catchment areas, river lengths, and volumes of deposited sediment that are consistent with the ranges observed in continental-scale deltas such as the Mississippi and Amazon rivers. (a) Example showing the outputs from the numerical simulation showing the elevation and bathymetry (top) and cumulative flexure (bottom). Model dimensions are 4500 km x 2000 km, with a vertical exaggeration of 100x. (b) Scatter plot of river length (top) and 405 shelf width (bottom) versus catchment area from river systems. Data is from Somme et al. (2009), Nyberg et al. (2018), Blum et al. (2013, 2017) and simulations presented in this study. Pal= Paleocene, Oli=Oligocene, PM= Paleo-Mississippi. (c) Example of synthetic stratigraphy from a simulation without (left) and with flexural compensation (right).  
  
**Animation:**  

Filename: [animation](https://github.com/ModelAtlasofTheEarth/model_submission/assets/29790931/b6dae5a4-f5bd-413d-ab7f-14349e1f54a1)  
Caption: The animation shows the surface and stratigraphic evolution of our simulated continental-scale deltas. We let each simulation initialize and run for 2 Myr without any sea-level fluctuations so that the delta can reach dynamic equilibrium without any disturbances in base level, then impose climate-forced sea-level changes.  
  
**Graphic abstract:**  

Filename: [egusphere-2023-53_Fig5.pdf](https://github.com/ModelAtlasofTheEarth/model_submission/files/15343754/egusphere-2023-53_Fig5.pdf)  
Caption: 
Output of numerical simulations with imposed synthetic sea-level curves with different frequencies (f) showing elevation, bathymetry and discharge of the river mouth at 8 Myr. Note the difference in lateral extent, elevation due to flexural rebound, and river mouth morphology between the flexural (top) and non-flexural (bottom) cases. (b) Change of river mouth location though time for simulations where synthetic and empirical sea-level curves were imposed. Mean river mouth transit distances in the non-flexurally compensated simulations are shown in lighter shades, whereas the flexurally compensated cases are shown in darker shades. (c) Bar plot showing the frequency of the number of times where the de-trended river-mouth trajectory crosses an arbitrary point in the shelf an indicator of how often the river mouth is close to the shelf break. NF = non-flexural, F = flexural, IH = icehouse, and GH = greenhouse.  
  
**Model setup figure:**  

Filename: [fig_setup.png](https://github.com/ModelAtlasofTheEarth/model_submission/assets/29790931/d28b8890-2681-4cd9-989b-424a119baba5)  
Caption:   
Description:  Planview of model setup (top) and cross-section in the middle of the modeling domain. The initial configuration of the modeling domain resembles the topography of a natural source-to-sink system with 3400 m elevation in the headwaters, a length of 4500 km, a downstream-decreasing fluvial channel slope, and successive inflections in gradient associated with the coastal-plain to continental shelf and shelf to slope transitions. To ensure that our simulated drainage basin produces a point-source for sediment input to the marine domain we imposed a longitudinal topographic low in the middle of the model.

  
