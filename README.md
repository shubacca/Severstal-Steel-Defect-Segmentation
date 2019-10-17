# Springboard Capstone Project 2: Severstal Steel Defect Image Segmentation 
The current project analyzes steel images obtained from <a href='https://www.kaggle.com/c/severstal-steel-defect-detection/overview'> Severstal databases </a>, and we are trying to develop a deep learning image segmentation model to correctly identify 4 types of defects on the images. Identifying different types of steel sheet defects is critical to improving the company's and industry's automation, increasing efficiency, and maintaining high quality in production. 

![](https://github.com/shubacca/Severstal-Steel-Defect-Segmentation/blob/master/Deliverables/severstal%20unmasked%20and%20masked%20images.png)

The train and test images, along with the sample submission and train files can be found <a href='https://www.kaggle.com/c/severstal-steel-defect-detection/data'> here. </a>

A Vanilla U-Net model has been used for the image segmentations task. Details on the report can be found <a href='https://github.com/shubacca/Severstal-Steel-Defect-Segmentation/blob/master/Deliverables/Milestone%20Report%202.pdf'> here. </a>

The Jupyter notebook associated with the project can be found <a href='https://nbviewer.jupyter.org/github/shubacca/Severstal-Steel-Defect-Segmentation/blob/master/Deliverables/Final%20Copy%20of%20Code.ipynb'> here. </a> 

The slide deck associated with this project is available <a href='https://github.com/shubacca/Severstal-Steel-Defect-Segmentation/blob/master/Deliverables/Slide%20Deck.pdf'> here. </a>

With the U-Net architecture, we were able to obtain a Sorenson-Dice coefficient of 0.680 for the train and validation data. The submission file containing the predictions for the test images can be downloaded from <a href='https://github.com/shubacca/Severstal-Steel-Defect-Segmentation/blob/master/Deliverables/submission.xlsx'> here </a>. To improve upon the existing U-Net model, many other changes can be made. The number of nodes per layer could be increased by a factor of 2, thus increasing the resolution of the trained weights. Another convolution and corresponding deconvolution layer can be added. A train-test split that was more representative of the defect distribution could have definitely improved the model accuracy and Dice coefficient. Other model architectures like FCNs, FPN, Mask R-CNN, ParseNet etc. could also have been used. 

Acknowledgement: <a href='https://www.kaggle.com/xhlulu/severstal-simple-keras-u-net-boilerplate'> xhlulu's boilerplate code </a> deserves credit for providing the skeleton for this code, over which I added in my own insights. 
