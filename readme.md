# Mask detection
<img src = "readme_images/elon.jpg" width = "400px" align = right>


## Dataset:  
https://www.kaggle.com/omkargurav/face-mask-dataset

## required librares:
- numpy
- pandas
- keras




## model:
- I used ResNet 50 and finetuned it after removing the last sofmax layer
- I added one more layer for two classes ["without_mask","withmask"]
- I used image data generator class in my model with no augmentation specified (I will maybe apply augmentation and see the difference)
- the model hyperparameters and loss function used could be found in the config cell [here](https://github.com/Ahmedmostafa2000/mask_detection_model/blob/main/Exploring_and_evaluating_best_model.ipynb)




<img src = "readme_images/example.jpg" width = "400px" align = right>

## results:
- the best model got an accuracy of 90% accuracy on training set, 93.5% accuracy on the developement set and 91% on the testing set  
- the model has a weak tendency to sky_blue objects such as towels, shirts and what so ever in the presence of a face (further investigation soon isa)  [I will put the unrecognized images in a folder]
- the model has a problem with differing between mask on a face and in picture, partially it would be addressed with face recog, but another issue arises which is a face with a mask but the face is not covered by the mask
- the model have the far face wearing mask issue, which also can be solved by using a face recognition before using the model  
- The model have a problem with detecting black masks in a large image

## Upcoming updates:

A readme update will be uploaded soon isa  
A demo will be uploaded soon  
A realtime implementation will be uploaded
A predict script will be uploaded
