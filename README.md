# Stereo-reconstruction

In this project, the 3d reconstruction of a scene is implemented using Naive Image patch approach, as well as the dynamic programming approach in the performance.xlsx file, the performance of the models over the dataset with different parameters is prwesented

The dataset used in the project is the middlebury dataset(2005-2006) from
https://vision.middlebury.edu/stereo/data/

According to the webpage, the focal length for the dataset is 3740 pixels and the baseline is 160 centimeters

the obtained disparity maps from the Naive approach, the DP algorithm and in built opencv SBM algorithm are
compared using SSD,MSQ and SSIM metrics.Also the runtime of all mentioned algorithms are stored in the excel file.

PSNR and SSIM metric calculatoin taken from :
SSIM
https://www.pyimagesearch.com/2017/06/19/image-difference-with-opencv-and-python/
PSNR
https://www.geeksforgeeks.org/python-peak-signal-to-noise-ratio-psnr/


screenshots of the 3d shapes recorded in Meshlab are available in data/Screenshots
