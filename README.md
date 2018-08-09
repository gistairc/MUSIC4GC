#  MUSIC for GC dataset

## Overview

According to [the census by R&A](https://www.randa.org/~/media/Files/DownloadsAndPublications/Golf-around-the-world-2017.ashx),  there are more than 30,000 golf courses all over the world.  They are good targets for research of automatic object detection due to their specific shape, world-wide distibution and common size.  **MUSIC** for GC (**G**olf  **C**ourse) is the dataset to support the global survey of golf courses based on satellite imagery.

First, we have created several KML files for polygons which cover all the golf courses in Japan. Next, [Landsat-8](https://landsat.usgs.gov/landsat-8) multiband images of these target areas were cropped into a 16 × 16 grids. These patch images are classified as “positives” if the golf course cover more than 20% of the total areas, while patches with no golf course are classified as “negatives”. The rest with the intermediate coverage (0~20%) were neither “positives” and “negatives”. 

![fig:MUSIC4GC image example](https://github.com/gistairc/MUSIC4GC/blob/master/fig0.png "Original polygons in a Landsat-8 scene")  


You can download the **MUSIC** for GC dataset from [here](http://data.airc.aist.go.jp/MUSIC4GC/MUSIC4GC.zip) (375MB).  More detailed exaplanations can be found in the following papers.

[1] *Uehara, K., H. Sakanashi, H. Nosato, M. Murakawa, H. Miyamoto, and R. Nakamura, “Object Detection of Satellite Images Using Multi-Channel Higher-order Local Autocorrelation”, IEEE International Conference on Systems, Man and Cybernetics
doi:10.1109/SMC.2017.8122799*


[2] *Miyamoto, H, K. Uehara, M. Murakawa, H. Sakanashi, H. Nosato, T. Kouyama and R.Nakamura,  "OBJECT DETECTION IN SATELLITE IMAGERY USING 2-STEP CONVOLUTIONAL NEURAL NETWORKS", [International Geoscience and Remote Sensing Symposium 2018] (https://www.igarss2018.org/Papers/viewpapers.asp?papernum=1645)*
         




## Download  

**IMPORTANT** -- Please read the [Terms of Use](https://github.com/gistairc/MUSIC4GC/blob/master/LICENSE.md) before downloading the MUSIC4P3 dataset.


#### How to extract 

The dataset can be downloaded from [here](http://data.airc.aist.go.jp/MUSIC4GC/MUSIC4GC.zip) (375MB) .  
Or type the following in the terminal.  

```
$ wget http://data.airc.aist.go.jp/MUSIC4GC/MUSIC4GC.zip
$ unzip MUSIC4GC.zip
```

The directory configuration in the unzipped folder:  
```
./MUSIC4GC/
train/
　　positive/
	LC81070302016189LGN00_point(66,232).tif
         LC81070302016189LGN00_point(67,232).tif ...
    negative/
         LC81070302016189LGN00_point(3,99).tif
         LC81070302016189LGN00_point(3,102).tif ...
val/
　　positive/
         LC81070302016189LGN00_point(69,233).tif
         LC81070302016189LGN00_point(188,158).tif ...
    negative/
         LC81070302016189LGN00_point(3,93).tif
         LC81070302016189LGN00_point(7,118).tif ...
test/
　　positive/
         LC81070302016189LGN00_point(73,236).tif
         LC81070302016189LGN00_point(73,237).tif ...
　　negative/
         LC81070302016189LGN00_point(3,101).tif
         LC81070302016189LGN00_point(4,103).tif ...
	
```

## Acknowledgement
This dataset and source code are based on results obtained from a project commissioned by the New Energy and Industrial Technology Development Organization (NEDO).  
