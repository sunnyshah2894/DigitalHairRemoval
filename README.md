# DigitalHairRemoval 

There has been numeruous advancements towards utilizing deep networks, ANNs, AI, etc in tasks like detecting the skin disease, type of tumour, etc. However, it becomes difficult for the networks to learn the features since, most of the skin images are occluded by hair. Thus, there is a need for pre-processing of the skin images to remove these obstructing hair. This sample project aims to remove the hair noise from the skin image with the help of Morphological filtering.

## Steps involved in the DHR algorithm

    - Convert the color image to a grayscale version. 
    - Applying Morphological Black-Hat transformation on the grayscale image
    - Creating the mask for InPainting task
    - Applying inpainting algorithm on the original image using the mask prepared from the grayscale image in step 3
    
## Examples:

### Example 1

| Original Image | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/inputImages/sample1.jpg) |
| ---      | ---       |
| GrayScaled Image | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/grayScale_sample1.jpg) |
| BlackHat filtering result     | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/blackhat_sample1.jpg) |
| Thresholded image for inpainting | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/thresholded_sample1.jpg) |
| Image after Inpainting| ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/InPainted_sample1.jpg) |


### Example 2

| Original Image | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/inputImages/sample2.jpg) |
| ---      | ---       |
| GrayScaled Image | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/grayScale_sample2.jpg) |
| BlackHat filtering result     | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/blackhat_sample2.jpg) |
| Thresholded image for inpainting | ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/thresholded_sample2.jpg) |
| Image after Inpainting| ![alt text](https://raw.githubusercontent.com/sunnyshah2894/DigitalHairRemoval/master/outputImages/InPainted_sample2.jpg) |

## Library

- Numpy
- OpenCV
