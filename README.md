# Fruit Inspection

Fruit inspection using classical computer vision techniques.

## First Task: Fruit Segmentation and Defect Detection

The aim of the first task is to correctly segment the fruit out of the given images, and then to detect the external defects of each fruit. To do so, the following steps have been taken:

- Image segmentation:
    1. The gray-level histogram of each image has been computed and then analyzed.
    2. Based on the result obtained at step i., a suitable thresholding method has been chosen.
    3. A flood-fill method has been used to fill the defect blobs of each image.
    4. Finally, the computed binary mask have finally been applied to the given images.


- Search for the defects in each fruit:
    1. Starting from the images obtained at step 1.D, a suitable edge detector has been used in order to find the edges of the different images.
    2. Given such edge masks, the original images have been modified so that external defects are finally highlighted.

The results of the first task are shown below:

![](https://i.ibb.co/pyrzsLm/1.png)

## Second Task: Russet Detection

The aim of the second task is to correctly detect the russet area in each fruit. To do so, the following steps have been taken:

- Image segmentation:
    1. The gray-level histogram of each image has been computed and then analyzed.
    2. Based on the result obtained at step i., a suitable thresholding method has been chosen.
    3. Finally, the computed binary masks have been applied to the given images.


- Search for the russet area in each fruit:
    1. Starting from the images obtained at step 1.C, four different colour spaces have been considered (RGB, HSV, HLS, LUV).
    2. A suitable colour distance has been used in order to segment the images and detect the russet area.
    3. Given the russet masks, the original images have been modified so that russet areas are finally highlighted.

The results of the second task are shown below:

![](https://i.ibb.co/S5TS2rt/2.png)

## Final Challenge: Kiwi Inspection

The aim of the third task is to correctly detect the defect area in image `C0_000007`. To do so, the following steps have been taken:

- Image segmentation:
    1. The gray-level histogram of each image has been computed and then analyzed.
    2. Based on the result obtained at step i., a suitable thresholding method has been chosen.
    3. The computed binary masks have been modified in order to eliminate the dirt located on the conveyor, as well as the sticker in image `C0_000006`.
    4. Finally, the computed binary masks have been applied to the given images.


- Search for the defect area:
    1. Starting from the images obtained at step 1.D, suitable masks have been computed so to detect defect areas in all the given images. The only defect such masks have to detect is the one in the afore-mentioned image (`C0_000007`).
    2. Given such binary masks, the original images have been modified so that the defect area is highlighted.

The results of the final challenge are shown below:

![](https://i.ibb.co/cbMtBwX/3.png)
