### -> submitter ORCID (or name)

0000-0002-1270-4377

### -> slug

polanco-2024-deltas

### -> license

CC-BY-4.0

### -> alternative license URL

_No response_

### -> model category

model published in study

### -> model status

completed

### -> associated publication DOI

10.5194/esurf-12-301-2024

### -> model creators


Sara Polanco (0000-0002-1270-4377)
0000-0003-0263-0084 
Tristan Salles ([0000-0001-6095-7689](http://orcid.org/0000-0001-6095-7689))
Frederick,Bruce C 
0000-0002-2594-6965
0000-0003-3693-932X
0000-0003-3566-1557
0000-0003-2595-2414
0000-0003-3685-174X


### -> title

_No response_

### -> description

Two-thirds of the world's most populated cities are situated close to deltas. We use computer simulations to understand how deltas sink or rise in response to climate-driven sea level changes that operate from thousands to millions of years. Our research shows that because of the interaction between the outer layers of the Earth, sediment transport, and sea level changes deltas develop a self-regulated mechanism that modifies the space they need to gain or lose land.

### -> abstract

_No response_

### -> scientific keywords

Flexural isostasy
Glacial isostatic adjustment (GIA)
Deltaic depocenters
Stratigraphic record

### -> funder

Australian Research Council, IH130200012
Australian–American Fulbright Commission
The University of Melbourne


### -> model embargo?

No

### -> include model code ?

- [X] yes

### -> model code/inputs DOI

10.5281/zenodo.10553849

### -> model code/inputs notes

The input and boundary conditions for the model are structured as follows:
an input XML file where the initial and boundary conditions are set
a data folder containing the initial surface and the boundary conditions, in this case different sea-level scenarios
a series of IPython Notebooks used to run the experiment and perform some pre or post-processing tasks.


### -> include model output data?

- [X] yes

### -> data creators

0000-0002-1270-4377

### -> model output data DOI

_No response_

### -> model output data notes

The model output data is stored in a hdf5 format. You will see a h5 folder and a series of xdmf files. 
- **h5** folder contains the **hdf5** data, all the information computed by the model are stored in these files. You will have at least the *tin* (surface) and *flow* (stream network) dataset and also the *sed* (stratigraphy) data if the stratal structure is computed in your simulation.

- two **.xdmf** files for the surface (**tin_series.xdmf**) and the flow network (**flow_series.xdmf**) that read the **xmf** files through time.

### -> model output data size

_No response_

### -> software framework DOI/URI

doi: 10.5281/zenodo.1069573

### -> software framework source repository

https://github.com/badlands-model/badlands

### -> name of primary software framework (e.g. Underworld, ASPECT, Badlands, OpenFOAM)

Badlands

### -> software framework authors

_No response_

### -> software & algorithm keywords

_No response_

### -> computer URI/DOI

_No response_

### -> add landing page image and caption

![fig1](https://github.com/ModelAtlasofTheEarth/model_submission/assets/29790931/166800c8-c053-4a04-a2ae-8526940e6f7b)
Our simulations produce catchment areas, river lengths, and volumes of deposited sediment that are consistent with the ranges observed in continental-scale deltas such as the Mississippi and Amazon rivers. (a) Example showing the outputs from the numerical simulation showing the elevation and bathymetry (top) and cumulative flexure (bottom). Model dimensions are 4500 km x 2000 km, with a vertical exaggeration of 100x. (b) Scatter plot of river length (top) and 405 shelf width (bottom) versus catchment area from river systems. Data is from Somme et al. (2009), Nyberg et al. (2018), Blum et al. (2013, 2017) and simulations presented in this study. Pal= Paleocene, Oli=Oligocene, PM= Paleo-Mississippi. (c) Example of synthetic stratigraphy from a simulation without (left) and with flexural compensation (right). 


### -> add an animation (if relevant)


https://github.com/ModelAtlasofTheEarth/model_submission/assets/29790931/b6dae5a4-f5bd-413d-ab7f-14349e1f54a1
The animation shows the surface and stratigraphic evolution of our simulated continental-scale deltas. We let each simulation initialize and run for 2 Myr without any sea-level fluctuations so that the delta can reach dynamic equilibrium without any disturbances in base level, then impose climate-forced sea-level changes.


### -> add a graphic abstract figure (if relevant)

[egusphere-2023-53_Fig5.pdf](https://github.com/ModelAtlasofTheEarth/model_submission/files/15343754/egusphere-2023-53_Fig5.pdf)

Output of numerical simulations with imposed synthetic sea-level curves with different frequencies (f) showing elevation, bathymetry and discharge of the river mouth at 8 Myr. Note the difference in lateral extent, elevation due to flexural rebound, and river mouth morphology between the flexural (top) and non-flexural (bottom) cases. (b) Change of river mouth location though time for simulations where synthetic and empirical sea-level curves were imposed. Mean river mouth transit distances in the non-flexurally compensated simulations are shown in lighter shades, whereas the flexurally compensated cases are shown in darker shades. (c) Bar plot showing the frequency of the number of times where the de-trended river-mouth trajectory crosses an arbitrary point in the shelf an indicator of how often the river mouth is close to the shelf break. NF = non-flexural, F = flexural, IH = icehouse, and GH = greenhouse.

### -> add a model setup figure (if relevant)

![fig_setup](https://github.com/ModelAtlasofTheEarth/model_submission/assets/29790931/d28b8890-2681-4cd9-989b-424a119baba5)

### -> add a description of your model setup

Planview of model setup (top) and cross-section in the middle of the modeling domain. The initial configuration of the modeling domain resembles the topography of a natural source-to-sink system with 3400 m elevation in the headwaters, a length of 4500 km, a downstream-decreasing fluvial channel slope, and successive inflections in gradient associated with the coastal-plain to continental shelf and shelf to slope transitions. To ensure that our simulated drainage basin produces a point-source for sediment input to the marine domain we imposed a longitudinal topographic low in the middle of the model. 

### Please provide any feedback on the model submission process?

Thanks Dan, great job!