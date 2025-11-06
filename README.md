# PLANT-DISEASE
# Why did i take this problem statement
This is my project for ML CA Submission. The source of the dataset is from kaggle. The dataset comprises of more than 3 lakh images distributed across 38 classes. Where the classes are as follows: apple healthy, apple diseasesd, pine healthy, pine diseased. Here i have tried to classify the Plant leaf as healthy or diseased for across 38 different species. Plant disease is a big concern because many plant diseases go undetected and they end up dying. Furthermore plant diseases can transfer from one plant to another plant. This is aimed so that timely detection of tree diseases can be donen and thus the plants can be saved!

# What was my thought Process
I started by uploading the dataset to prepare it for the EDA. Where i find out a particular plant in the dataset also has the respective diseases associated with it, meaning Apple Healthy and then we have Apple has disease Black Rot, Apple has disease scab and so on. I then found out the distribbution of images across all 38 classes to check whether the data was imbalanced? meaning whether one class of data had more images than the other? because this would have lead to bias.Fortunately the dataset was not very imbalanced and only had differences in the range of 1k or 2k.
I then went on to visualize the leaves to see how they really look to actually visually get a understanding of what a healthy vs an infected leaf looked like. 

I then plotted a RGB value histogram(Red Green Blue) for both healthy as well as a disease leaf for a partiular plant. I repeated this for multiple plant species to strengthen my conclusion:
Healthy leaves generally show balanced, mid-range RGB peaks, while diseased ones (like scab or blight) show shifts to lower intensities, indicating darker patches and lesion areas.
These pixel intensity differences confirm that color is a strong signal for classification.

# Model Selection
So i decided that i will not convert to grayscale as i had strong evidence that the color of the leaf was an  important factor.

I then applied CNN for 10 epochs where i achieved an accuracy of 93%.
I also applied MobileNetV2 as my second model.

The graphs of loss as well as accuracy for both of these models can be found in the colab ipynb file attached.

