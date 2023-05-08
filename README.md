# YOLO Drone Detection

This repository contains the code for training and running a YOLOv7 object detection model for detecting drones in images.

## Getting Started

Follow the steps below to set up the project and run the Jupyter notebook:

### 1. Create a project folder

Create a folder for the project files. This folder is called `PROJECT_ROOT` from now on. Two git projects and a virtual environment will be stored here.

### 2. Clone the project

git clone https://github.com/Iddo77/YOLO_drone_detection.git

### 3. Clone the YOLO v7 project

git clone https://github.com/WongKinYiu/yolov7.git

### 4. Download pretrained YOLO model

Download: https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7_training.pt

Save the model in the `yolov7` folder.

### 5. Set up a virtual environment

Run the following commands from `PROJECT_ROOT`:

python -m venv yolo-drones-env
<yolo-drones-env>\Scripts\activate

### 6. Install PyTorch with CUDA

Check the version of CUDA that you are running. Go to the PyTorch website and look up the command to install a CUDA-enabled version of PyTorch. Running this project without CUDA is not possible.

### 7. Install YOLO v7 requirements

Use the command line application with the activated virtual environment. Navigate to the `yolov7` folder and run:

pip install -r requirements.txt

### 8. Install and run Jupyter Notebook

pip install jupyter
jupyter notebook

In the browser that opens, choose 'upload' and select `YOLO_drones.ipynb` from the `YOLO_drone_detection` folder. Set the `PROJECT_ROOT` variable in the 3rd cell to the `PROJECT_ROOT`.

**Note**: When you want to commit changes to `YOLO_drones.ipynb` made in Jupyter, you must first copy the file back to the original location.

## Running the Code

setting up the project, you can run the code in the Jupyter notebook to train and evaluate the YOLOv7 object detection model for drone detection. The results will be stored in the folder `<PROJECT_ROOT>/yolov7/runs/train/yolov7-custom<index>` (index is a number that is incremented every time you run it).



