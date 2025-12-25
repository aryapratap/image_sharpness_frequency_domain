# image\_sharpness\_frequency\_domain



This notebook will present a methodology to quantify image sharpness using the frequency domain of the image. With varying focus positions or different focal lengths, different parts of an image are being focused, resulting in highlighting certain frequencies at a time while making the rest blurred. This method will highlight sharp features only. This will be helpful in 2 ways primarily. First is if the overall image is sharp or not. We can compare the component of the remaining frequencies after applying the high pass filter to see what is the total magnitude of frequencies remaining, or instead the total pixels that have the high frequencies. Second is using this as a cost function in deep leanring neural networks where spatial integrity is something that needs to be checked like boundary detection, object segmentation, preferably in the Unet architectures.



The test data is from : https://github.com/bznick98/Focus\_Stacking/tree/master/assets/test\_images



Sharpness original code inspiration : 
https://stackoverflow.com/questions/58392838/how-to-get-information-about-sharpness-of-image-with-fourier-transformation

