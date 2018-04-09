# Assignment-2 : Huzaifa Abbasi, 14CO216

Part - 1:
Segment the images to find the lesions in the dataset. For this the U-Net architecture is used which has been proven to be effective in medical image segmentation.  
The network has been trained with 1800 images and validated with 200 images.  
**Mean_IOU score = 0.8023**  
**Dice Coefficient = 0.8529**  
**Accuracy = 0.9696**  
The code is available in `Segmentation.ipynb`

Part - 2:
Classify the images into Melanoma(1) and Other(0) classes. Since this dataset is skewed towards the negative class ( 18% of Melanoma images and 82% of non_melanoma images ), f1-score instead of accuracy has been used to evaluate the performance.
To handle the skewness, class weights have been used to give more importance to the Melanoma class.  
The **f1-score on Melonoma = 0.144**  
The **f1-score on Other = 0.777**  
The code is available in `Classification.ipynb`
