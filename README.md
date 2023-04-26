# Object-Tracking-System-using-DeepSORT

In order to install the reuirements, use the commands below
# Tensorflow CPU
conda env create -f conda-cpu.yml

conda activate tracker-cpu

OR use pip

pip install -r requirements.txt

# Load the weights
In order to load the weights and convert into a tensorflow model,

python load_weights.py
# yolov3 on the model
In order to run the object tracker for the model, use the following commands depending on your input is recorded or a webcam.

#yolov3 on video

python object_tracker.py --video ./data/video/test.mp4 --output ./data/video/results.avi

#yolov3 on webcam 

python object_tracker.py --video 0 --output ./data/video/results.avi
