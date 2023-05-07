# YOLO Drone Detection

This repository contains the code for training and running a YOLOv7 object detection model for detecting drones in images.

## Getting Started

Follow the steps below to set up the project and run the Jupyter notebook:

### 1. Clone the project

git clone https://github.com/Iddo77/YOLO_drone_detection.git


### 2. Set up a virtual environment

python -m venv yolo-drones-env
copy YOLO_drones.ipynb yolo-drones-env\Scripts
cd yolo-drones-env\Scripts
activate


### 3. Install and run Jupyter Notebook

python.exe -m pip install --upgrade pip
pip install jupyter
jupyter notebook

In the browser that opens, select `YOLO_drones.ipynb`.

**Note**: When you want to commit changes to `YOLO_drones.ipynb` made in Jupyter, you must first copy the file back to the original location.

### 4. Install PyTorch with CUDA support (if needed)

If CUDA is not found, follow these steps:

- Exit the Jupyter notebook if it is started.
- Make sure you start the command line as admin.
- Activate the virtual environment and go to the `yolov7` folder.
- Uninstall the existing PyTorch packages:

pip uninstall torch torchvision torchaudio

- Install the appropriate PyTorch packages for your CUDA version:
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117

#### Download Pre-trained YOLOv7 Model

1. Download the pre-trained YOLO v7 base model by clicking on the following link: [yolov7_training.pt](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7_training.pt)

   Full URL: `https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7_training.pt`

2. Place the downloaded `yolov7_training.pt` file in the `yolov7` folder.



## Running the Code

After setting up the project, you can run the code in the Jupyter notebook to train and evaluate the YOLOv7 object detection model for drone detection.



