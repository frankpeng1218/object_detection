# object_detection
![image](https://github.com/user-attachments/assets/f9c7d1b6-e164-437e-900b-240bc7f57a52)

**Kaggle:** a popular platform for data science and machine learning enthusiasts. Kaggle hosts datasets from various domains, making it easier for users to access real-world data for analysis, visualization, and building machine learning models.

![image](https://github.com/user-attachments/assets/bda0a13e-9177-4626-b5d0-c5468077f886)

**Roboflow:** a platform designed to simplify the development of computer vision models for robotics, automation, and related applications. RobotFlow typically focuses on datasets, models, and tools that cater to robotics and computer vision tasks like object detection, segmentation, and classification.

1. Users can download the open-source image dataset from Kaggle and annotate/label these images in Robotflow. Additionally, users can upload video for dataset as well. In the Robotflow, there are auto-label and manually label users can use.
2. After finishing the labeling, we can generate the pre-processing images.

The application is applied on the Jetson Nano 2GB Developer Kit platform
**Jetson nano setup:**  
The way to setup jupyter path: https://blog.csdn.net/qq_25662827/article/details/122158526
The way to install oled display with ip and memory usage: https://www.youtube.com/watch?v=eMNIfNaSHQY


```
sudo docker pull python:3.12
sudo docker images
sudo docker run --gpus all -it -v /home/jetson-nano/yolo_12242024:/yolo_12242024 python:3.12 bash
apt update
apt install -y libgl1 libglib2.0-0
pip install --upgrade pip setuptools wheel
pip install ultralytics
pip install roboflow

```



3. We can train the model through Robotflow. However, after downloading the dataset, we'll get the api key and train the model on our side.
4. Go to colab to train the model 
