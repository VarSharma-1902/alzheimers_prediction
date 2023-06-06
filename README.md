# alzheimers_prediction

In order to assess whether a person has Alzheimer's disease or not, we create a detection model that employs image segmentation to spot changes in MRI images. 
If the model indicates that Alzheimer's disease is present, it will also indicate the patient's current illness stage. Different deep-learning models are used here. <br><br>
We use deep learning models to learn patterns in the segmented images that correspond to specific changes of interest like the change in brain size and other parts observed 
due to Alzheimer's disease. The models are trained on a set of labels, where the images are first enhanced using different filters such as Gaussian filter and unsharp filter, 
and Histogram eequalization However, to study how the efficiency of the model differs on applying various filters, we have trained and tested our models in different 
scenarios using images with and without the filters. <br><br>
It was observed that sufficiently good results were obtained when our proposed CNN model was trained on the original dataset and the 
MRI scan images after applying the unsharp filter. <br><br>
We get the best accuracy when the unsharp filter is applied to the images and trained on the 2nd CNN model, a good train, validation, and test accuracy was observed 
without any overfitting or underfitting. The same applies to the original dataset as well when trained using the CNN models. 
Hence, we can either choose the two CNN models with the original dataset or, we can apply the unsharp filter on the images first and then use the 2nd CNN model.
