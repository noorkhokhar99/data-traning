# data-traning

The Pothole Detection Dataset to Train YOLOv8

We are using quite a large pothole dataset in this article which contains more than 7000 images collected from several sources.

Download the Dataset

If you plan to execute the training commands on your local system, you can download the dataset by executing the following command.



````
wget https://www.dropbox.com/s/qvglw8pqo16769f/pothole_dataset_v8.zip?dl=1 -O pothole_dataset_v8.zip
````

Next, unzip it in the current directory.

unzip pothole_dataset_v8.zip

Inside the directory, we are the dataset is contained in the train and valid folders. As with all other YOLO models, the labels are in the text files with normalized xmin, ymin, width, height.

Setting Up YOLOv8 to Train on Custom Dataset


To train YOLOv8 on a custom dataset, we need to install the ultralytics package. This provides the yolo Command Line Interface (CLI). One big advantage is that we do not need to clone the repository separately and install the requirements.

Note: Before moving further into the installation steps, please install CUDA and cuDNN if you want to execute the training steps in your system.
We can install the package using pip.

````
pip install ultralytics
````

Setting Up ClearML

````
pip install clearml
````


script for Training YOLOv8 on Custom Dataset


