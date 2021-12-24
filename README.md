# Stereo-reconstruction
# Parsa Pourzargham Neptun ID: LUM2CE

In this project, the 3d reconstruction of a scene is implemented using Naive Image patch approach, as well as the dynamic programming approach in the performance.xlsx file, the performance of the models over the dataset with different parameters is presented

The dataset used in the project is the middlebury dataset(2005-2006) from
https://vision.middlebury.edu/stereo/data/

According to the webpage, the focal length for the dataset is 3740 pixels and the baseline is 160 centimeters

the obtained disparity maps from the Naive approach, the DP algorithm and in built opencv SBM algorithm are
compared using SSD,MSQ and SSIM metrics.Also the runtime of all mentioned algorithms are stored in the excel file.

PSNR and SSIM metric calculation is done with a python script seperately.Code for SSIM and PSNR taken from :

SSIM

https://www.pyimagesearch.com/2017/06/19/image-difference-with-opencv-and-python/

PSNR

https://www.geeksforgeeks.org/python-peak-signal-to-noise-ratio-psnr/


screenshots of the 3d shapes recorded in Meshlab are available in data/Screenshots

Main image 

![view1](https://user-images.githubusercontent.com/72257286/142197666-8e938429-14f3-4abc-bb27-819bd87f7bfe.png)

Ground truth Disparity map

![disp1](https://user-images.githubusercontent.com/72257286/142197597-7a58dc91-6f15-44e4-87b6-5cc41c48bccc.png)


DP Disparity map

![output-dp-disparity](https://user-images.githubusercontent.com/72257286/142197692-9ff9785a-78bf-40ca-93e7-fb3a960b7bf5.png)


Naive approach Disparity map 

![output-naive-disparity](https://user-images.githubusercontent.com/72257286/142197734-35c0efdf-da19-4d3a-bfe4-6c69addfd971.png)

3D results 

3D model generated with the ground truth disparity:

![Aloe GT](https://user-images.githubusercontent.com/72257286/147368753-0c2afbb9-185e-4d9b-a60f-621e074eb8be.png)

![Midd1 GT](https://user-images.githubusercontent.com/72257286/147369050-64aca4a4-bdc4-4168-91c3-5cce40089bd4.png)

![Moebius GT](https://user-images.githubusercontent.com/72257286/147369057-6c38477c-6384-4166-afa8-8fa1925bc53d.png)



3D model generated withDynamic programming disparity:

![Aloe dp](https://user-images.githubusercontent.com/72257286/147368757-93a2e3df-7dd7-49e8-9f6e-375b2c742e1d.png)

![Midd1 dp](https://user-images.githubusercontent.com/72257286/147369067-81b6d649-68f5-4680-b16a-700a968aaa77.png)

![Moebius dp](https://user-images.githubusercontent.com/72257286/147369071-da1c561f-8738-4ead-9a59-b7dd9dfef2e7.png)



3D model generated with the Naive approach disparity:

![Aloe naive](https://user-images.githubusercontent.com/72257286/147368761-cfdd239e-33c3-4124-9a78-0ed9af446e9b.png)

![Midd1 Naive](https://user-images.githubusercontent.com/72257286/147369079-d6592bca-8aa7-489c-9f77-a3ada719b4f0.png)

![Moebius Naive](https://user-images.githubusercontent.com/72257286/147369084-9875fb5e-7f76-4196-896c-0e1a3ee43c8a.png)




3D model generated with SBM disparity:

![Moebius SBM](https://user-images.githubusercontent.com/72257286/147369090-22b48d14-4e3c-41dc-b630-b57c96b2a4e0.png)


Difference images:

here are the difference images compaerd to ground truth:

Naive:

![NAIVE Difference](https://user-images.githubusercontent.com/72257286/147368833-e40c8c28-6930-4fc7-9d8e-8ad314828600.png)


DP:

![Dynamic programming Difference](https://user-images.githubusercontent.com/72257286/147368837-2d774a5f-a2e2-4f6b-a79b-559f2bd86ebc.png)


SBM:

![SBM Difference](https://user-images.githubusercontent.com/72257286/147368843-b4201e16-f75a-4d32-8375-d2cfe5995335.png)





