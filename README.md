# dissertation_code
All Python code produced for my dissertation on classifying Scottish peatland conditions from Sentinel-2 data. This includes sampling Sentinel-2 data, then separating the data into different notebooks for multi-class and binary classifications. 

The folders named by year (2017-2023) contain individual sampling datasets for the peatland conditions present in those years. In 2017, for example, only one dataset was made corresponding to the one peatland condition sampled for a single AOI, whereas for 2018, several datasets were made corresponding to both different peatland conditions and different AOIs (each dataset is named accordingly).

The 'peatland_sampling_2018_example.ipynb' is the notebook template used to create all sampling datasets, though the one included here shows specifically the data for 2018 AOI 1 where only 'bare peat' (class 3) was present. 

The 'combining_datasets_ipynb' shows the process of merging all sampling datasets into one large dataset. Due to the size of the combined_df (which is also sometimes called merged_df), it was not possible to upload it here. 

The 'training_and_evaluating_rx_nx.ipynb' are here uploaded for each classification performed for the project, where r1 (round 1) classifications are multi-class, and the rest of the classifications are binary variations. For each round, the first classification (classification 1, 3, 5, 7 and 9) are based on only Sentinel-2 bands B1-B12, and the second classification (classification 2, 4, 6, 8 and 10) are based on B1-B12 and vegetation indices (NDVI, EVI, NDWI, SAVI and GNDVI). The datasets are configured accordingly in each notebook to either include or exclude vegetation indices, and classes are collapsed or excluded for the binary classifications 3-10.

Lastly, the 'vi_plots.ipynb' notebook show how vegetation index distributions across classes were made for the multiclass dataset, as well as some other, general EDA. 
