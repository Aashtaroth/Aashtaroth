# Jetson AI Specialist Project: Gesture-task Mapping
This project builds on the image classification format provided by Nvidia's Jetson nano AI course on Jupyter notebook and uses a model trained from it
to link each image category (hand gestures) to a set of tasks (display certain images) to be triggered and performed immediately.

# Procedures
1. ssh with a usb address into a Jetson Nano device, then launch the Nvidia docker container:
sudo docker run --runtime nvidia -it --rm --network host \
    --volume ~/nvdli-data:/nvdli-nano/data \
    --device /dev/video0 \
    nvcr.io/nvidia/dli/dli-nano-ai:v2.0.1-r32.6.1

2. Access the Jupyter Notebook http://192.168.55.1:8888/lab?
3. Under 'data' directory, copy all the files in this repository.
4. Launch 'classification_interactive.ipynb' and execute each cell commands in order.
5. Train your own gestures/symbols/signs.
6. Execute the image-displaying script at the bottom.

# Tutorial Video
https://www.youtube.com/watch?v=5PRwjeiIGBg






