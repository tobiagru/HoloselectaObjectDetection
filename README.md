# ObjectDetection
ObjectDetection for Grocery Products. These are the files as part of the publication: https://www.researchgate.net/profile/Klaus_Fuchs2/publication/337068624_Towards_Identification_of_Packaged_Products_via_Computer_Vision_Convolutional_Neural_Networks_for_Object_Detection_and_Image_Classification_in_Retail_Environments/links/5dc7de0692851c81803f4126/Towards-Identification-of-Packaged-Products-via-Computer-Vision-Convolutional-Neural-Networks-for-Object-Detection-and-Image-Classification-in-Retail-Environments.pdf

The data sets can be obtained at: https://github.com/tobiagru/ObjectDetectionGroceryProducts

## Explanation
The research was seperated into two parts. Checking pure classificaiton performance and checking object detection performance. Everything was written in Colab. Thus it is easiest to copy this repository to your Google Drive and open the files in Colab.

### Classification 
Both files include all the required loaders and tools, the difference is how the algorithm is tuned. V1.2 only traines the classification layer, while V2.0 finetunes the entire network. 

The classification is based on networks from tensorflow hub and the entire algorithm is built in Keras.

### Object Detection
Object Detection is based on the Google Research Object Detection API.

#### Data
The labeling was done with labelImg (https://github.com/tzutalin/labelImg) but CleanData can be used to adjust the labels per individual patch. The major tool is Create Dataset which can be used to turn the dataset into TFRecords files as required for the Object Detection API.

#### Training
The training folder contains different scripts for different training platforms. Not all models can be trained on TPU thus there are GPU and TPU versions. On top due to the fact that one can only run one GPU Colab but I needed multiple there are as well files to train on the Google Cloud with the Machine Learning Engine.

#### Export
Export are tools to export the models to various platforms. TFLite for Android Apps, Unity for Baracuda based Apps, Serving for Tensorflow Extended Serving. Inference Colab can be used to upload files and make predicitons in Colab. 
