---
layout: default
title: The Canadian Cropland Dataset
nav_order: 1
---

# Description

The *Canadian Cropland Dataset* is a temporal patch-based dataset of remote sensing images of Canadian croplands retrieved from the Sentinel-2 satellite constellation. The dataset contains 78,536 manually verified and curated high-resolution (10 m/pixel, 640 x 640 m) geo-referenced images from 10 crop classes collected over four crop production years (2017-2020) and five months (June-October) which were extracted using [Google Earth Engine](https://earthengine.google.com/  "Google Earth Engine") (GEE) and were automatically labelled with the [Canadian Crop Inventory](https://www.agr.gc.ca/atlas/aci "Canadian Crop Inventory") Each instance contains 12 spectral bands, an RGB image, and additional vegetation index bands. Individually, each crop category contains at least 4,800 samples.


<p align="center"><img src="figures/home/crop_mosaic_10_categories.png" alt="An overview of sample patches of the crop classes in the dataset. The images measure 64 x 64 pixels and have a spatial resolution of 10 m/pixel." width="980" height="495" /></p>

**Keywords :** satellite imagery, remote sensing, dataset, agriculture, cropland, supervised learning, image classification, deep learning.

___

## Key Features


#### **Multitemporal remote sensing dataset spanning multiple years** 
 {: .text-red-300 }   
 - More than 70% of geolocations have an image collection of at least 10 images (over 4 years), allowing a temporally rich monitoring of a field through a multi-year, multi-crop rotation

#### **Transformed .PNG images ready to be directly used with deep learning benchmarks** 
{: .text-red-300 }
- Each field instance contains an RGB image as well as common vegetation index images (NDVI, NDVI45, GNDVI, OSAVI and PSRI; NDWI is inluded in the 2020 version and on) in .PNG format.

#### **High spectral resolution images** 
 {: .text-red-300 }
 - We also supply a .zip folder with the original Sentinel-2 bands (12) and 6 additional vegetation index bands as georeferenced .TIF files. 

#### **Pre-constructed train / val / test sets** 
{: .text-red-300 }
- The dataset comes prepackaged in dedicated training (70%), validation (15%) and testing sets (15%) suitable for use with Keras or Tensorflow image data generators. These sets remain the same for each individual year and image type (i.e NDVI, PSRI, etc.). Images belonging to the same geographical coordinates were kept together during the dataset splitting process

___

## Download Link

Both the cleaned and RAW versions of the dataset and can be downloaded from this [Google Drive ](https://drive.google.com/drive/folders/1mNI8B5EMk0Xgvx2Pc9ztnQRaW9pXh8yb?usp=sharing "Link to dataset") link. 

___

## Citation

```
@misc{boatswainjacques2023canadian,
      title={The Canadian Cropland Dataset: A New Land Cover Dataset for Multitemporal Deep Learning Classification in Agriculture}, 
      author={Amanda A. {Boatswain Jacques} and {Abdoulaye Baniré} Diallo and Etienne Lord},
      year={2023},
      eprint={2306.00114},
      archivePrefix={arXiv},
      primaryClass={cs.CV}}
```
___

## License 

**The dataset** is released under the [*Montreal Data License*](https://github.com/bioinfoUQAM/Canadian-cropland-dataset/blob/main/DATA_LICENSE) which is a [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) creative commons license. 
**The software** for benchmarking is available under the [MIT](https://github.com/bioinfoUQAM/Canadian-cropland-dataset/blob/main/CODE_LICENSE) license.

{: .warning }

The dataset is available for individuals, researchers, principal investigators and government workers. It is derived from Google Earth Engine and is subject to its terms. Thefore, **this dataset is to be used purely for discovery and not for commercial purposes.**

___
