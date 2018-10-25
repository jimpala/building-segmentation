# satellite-segmentation

This is a repository with a TensorFlow implementation of a U-Net satellite image segmentation model, based upon the Kaggle *DSTL Satellite Imagery Feature Detection* competition. Further documentation is forthcoming.

This model particularly focuses on performance for segmentation of buildings in the satellite images. An example figure demonstrating segmentation performance is shown below, with test image on the right, and prediction on the left (white pixels corresponding to building predictions, black prixels corresponding to non-building predictions).

![Image placeholder](https://s3.eu-west-2.amazonaws.com/jpyne17-github-media/building_detection.png)

## Kaggle Competition Info

In this Kaggle competition, DSTL provides 1km x 1km satellite images in both 3-band and 16-band formats. The goal is to detect and classify the types of objects found in these regions.

There are two types of imagery in this analysis. The 3-band images are the traditional RGB natural color images. The 16-band images contain spectral information by capturing wider wavelength channels. This multi-band imagery is taken from the multispectral (400 – 1040nm) and short-wave infrared (SWIR) (1195-2365nm) range.

In each satellite image, there are lots of different common objects like roads, buildings, vehicles, farms, trees, waterways, etc. DSTL has labeled 10 different classes:

- Buildings - large building, residential, non-residential, fuel storage facility, fortified building.
- Misc. manmade structure.
- Road.
- Track - poor/dirt/cart track, footpath/trail.
- Trees - woodland, hedgerows, groups of trees, standalone trees.
- Crops - contour ploughing/cropland, grain (wheat) crops, row (potatoes, turnips) crops.
- Waterway.
- Standing water.
- Vehicle Large - large vehicle (e.g. lorry, truck,bus), logistics vehicle.
- Vehicle Small - small vehicle (car, van), motorbike.