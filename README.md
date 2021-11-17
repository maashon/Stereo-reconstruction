# Stereo-reconstruction

In this project, the 3d reconstruction of a scene is implemented using Naive Image patch approach, as well as the dynamic programming approach in the performance.xlsx file, the performance of the models over the dataset with different parameters is prwesented

The dataset used in the project is the middlebury dataset(2005-2006)

https://vision.middlebury.edu/stereo/data/

According to the webpage, the focal length for the dataset is 3740 pixels and the baseline is 160 centimeters

the obtained disparity maps from the Naive approach, the DP algorithm and in built opencv SBM algorithm are
compared using SSD,MSQ and SSIM metrics.Also the runtime of all mentioned algorithms are stored in the excel file.

PSNR metric calculatoin taken from :

https://www.ccoderun.ca/programming/doxygen/opencv_3.2.0/tutorial_gpu_basics_similarity.html
