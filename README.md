## Digital Image Enhancement, Restoration and Object Segmentation Using the Oxford-IIIT Pet Dataset

## Project Description 
 
This project focuses on digital image enhancement, noise restoration, edge detection, and object segmentation using the Oxford-IIIT Pet Dataset. 
 
Spatial and morphological image processing techniques are applied to improve image quality, remove noise, detect object boundaries, and separate the pet from the background. 
 
## Objectives 
 
- Preprocess pet images for image processing. 
- Improve image quality using enhancement techniques. 
- Study Gaussian and salt-and-pepper noise. 
- Remove noise using mean, median, and Wiener filtering. 
- Detect object boundaries using Sobel and Canny edge detection. 
- Segment the pet using Otsu thresholding. 
- Improve segmentation using morphological operations. 
- Compare segmentation results with the ground-truth mask. 
- Evaluate restoration using MSE, PSNR, and SSIM. 
- Evaluate segmentation using IoU, Dice Score, and Accuracy. 
 
## Dataset 
 
The project uses the **Oxford-IIIT Pet Dataset**. 
 
The dataset contains images of different breeds of cats and dogs along with segmentation annotations. 
 
The dataset is loaded using the `OxfordIIITPet` dataset available in Torchvision. 
 
Images are resized to **256 × 256 pixels**, and RGB images are converted into grayscale for intensity-based image processing. 
 
## Methodology 
 
The project follows the workflow: 
 
**Input Image → Preprocessing → Image Enhancement → Noise Addition → Noise Removal / Restoration → Edge Detection → Segmentation → Morphological Post-processing → Ground Truth Comparison → Evaluation** 
 
## Techniques Used 
 
### Image Enhancement 
 
- Gamma Transformation 
- Contrast Stretching 
- Histogram Equalization 
 
### Noise Addition 
 
- Gaussian Noise 
- Salt-and-Pepper Noise 
 
### Noise Restoration 
 
- Mean Filtering 
- Median Filtering 
- Wiener Filtering 
 
### Edge Detection 
 
- Sobel Edge Detection 
- Canny Edge Detection 
 
### Segmentation 
 
- Otsu Thresholding 
 
### Morphological Processing 
 
- Erosion 
- Dilation 
- Opening 
- Closing 
 
## Evaluation Metrics 
 
### Restoration 
 
- Mean Squared Error (MSE) 
- Peak Signal-to-Noise Ratio (PSNR) 
- Structural Similarity Index (SSIM) 
 
### Segmentation 
 
- Intersection over Union (IoU) 
- Dice Score 
- Accuracy 
 
## Technologies Used 
 
- Python 
- NumPy 
- OpenCV 
- Matplotlib 
- Pandas 
- Torchvision 
- SciPy 
- scikit-image 
 
## Results


The project produces results for:

Image enhancement
Gaussian and salt-and-pepper noise
Noise restoration
Sobel and Canny edge detection
Otsu segmentation
Morphological processing
Ground-truth comparison

Restoration results are evaluated using MSE, PSNR, and SSIM. Segmentation results are evaluated using IoU, Dice Score, and Accuracy.

## Limitations
Otsu thresholding may not work well when the pet and background have similar intensity values.
Edge detection may not detect complete object boundaries.
Restoration performance depends on the noise level and filter size.
Traditional image processing techniques may not recover details that are completely lost.
The project uses a selected number of images for processing.

## Future Scope
Use a larger and more diverse set of images.
Apply adaptive filtering techniques.
Use adaptive thresholding and watershed segmentation.
Explore frequency-domain filtering.
Apply deep learning-based image segmentation.
Perform evaluation on a larger number of images.
Develop a real-time image processing application.

## Conclusion

This project demonstrates the use of spatial and morphological image processing techniques for image enhancement, noise restoration, edge detection, and object segmentation. The results are evaluated using both quantitative metrics and visual comparison with ground-truth masks.
