#  MUSIC for GC dataset

## Overview

According to [the census by R&A](https://www.randa.org/~/media/Files/DownloadsAndPublications/Golf-around-the-world-2017.ashx),  there are more than 30,000 golf courses all over the world.  They are good targets for research of automatic object detection due to their specific shape, world-wide distibution and common size.  **MUSIC** for GC (**G**olf  **C**ourse) is the dataset to support the global survey of golf courses based on satellite imagery.

First, we have picked up all golf courses in Japan imaged by Landsat-8 between 200? and 200?. Their profile are represented as polygons and the longitude/latitude of each point is stored in KML files. Next, [Landsat-8](https://landsat.usgs.gov/landsat-8) multiband images of these target areas were cropped into a 16 × 16 grids, which corresponds to a 480 × 480 meter area. These patch images are classified as “positives” if the golf course cover more than 20% of the total areas, while patches with no golf course are classified as “negatives”. The rest with the intermediate coverage (0~20%) were neither “positives” and “negatives”. 

![fig:MUSIC4GC image example](https://github.com/gistairc/MUSIC4GC/blob/master/fig0.png "Original polygons in a Landsat-8 scene")  


You can download the **MUSIC** for GC dataset from [here ]( ????? ) (??GB).  More detailed exaplanations can be found in the following papers.

[1] *Uehara, K., H. Sakanashi, H. Nosato, M. Murakawa, H. Miyamoto, and R. Nakamura, “Object Detection of Satellite Images Using Multi-Channel Higher-order Local Autocorrelation”, IEEE International Conference on Systems, Man and Cybernetics
doi:10.1109/SMC.2017.8122799*


[2] *Miyamoto, H, K. Uehara, M. Murakawa, H. Sakanashi, H. Nosato, T. Kouyama and R.Nakamura,  "OBJECT DETECTION IN SATELLITE IMAGERY USING 2-STEP CONVOLUTIONAL NEURAL NETWORKS", [International Geoscience and Remote Sensing Symposium 2018] (https://www.igarss2018.org/Papers/viewpapers.asp?papernum=1645)*
         




## Download  

**IMPORTANT** -- Please read the [Terms of Use](https://github.com/gistairc/MUSIC4GC/blob/master/LICENSE.md) before downloading the MUSIC4P3 dataset.


#### How to extract 

The dataset can be downloaded from [here](http://data.airc.aist.go.jp/MUSIC4P3dataset/MUSIC4P3data_hdf.zip) (4.6GB) .  
Or type the following in the terminal.  

```
$ wget http://data.airc.aist.go.jp/MUSIC4GCdataset/????????????
$ unzip ????????????
```

The directory configuration in the unzipped folder:  
```
ここも入れてください。	
``

## Acknowledgement
This dataset and source code are based on results obtained from a project commissioned by the New Energy and Industrial Technology Development Organization (NEDO).  
