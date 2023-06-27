# facemask-detection
facemask  detection  it tell you how many are using mask  and  how many are not using it 

This model checks if a person is wearing face-mask or not.
It detects faces using OpenCV.
Classification is done using Deep-Learning Model.
The model contains Tensorflow-Keras and CNN Layers.

The dataset used to train the model contains 12,000 images.
Link to the dataset:https://www.kaggle.com/datasets/srikarimalladi/face-mask-detection-12k-images-dataset/code?datasetId=3454882&sortBy=dateRun&tab=profile


This TensorFlow face mask detection model has been deployed using a Podman Docker image and Flask API. To run the Podman image on your Windows local machine, follow the steps below:

Install Podman on your local machine. Download and install the MSI file from the 'Assets' section of the latest version of Podman.
After you have installed Podman, create a new virtual machine that runs the Podman container engine by entering this command in your Windows PowerShell: podman machine init.
Start the virtual machine by running this command: podman machine start.
Pull the Podman image from GitHub Packages by running the following command: podman pull ghcr.io/SrikariMalladi/fmd:1. The size of this image is 1.79 GB.
Run the Podman container using the following command: podman run -p 8888:5000 ghcr.io/SrikarMalladi/fmd:1.
You should be able to access the API by visiting http://localhost:8888 in your web browser.
You can remove the image using the command: podman rmi ghcr.io/SrikariMalladi/fmd:1 or podman rmi --force ghcr.io/SrikariMalladi/fmd:1.
