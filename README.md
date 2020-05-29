# Cat detector

Raspberry pi tools for cat detection with tensorflow. These tools extend the
work presented by Evan at:

- https://github.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi

- https://www.youtube.com/watch?v=aimSGOAUI8Y&t=482s



## Introduction


## Hardware

Hardware used for this project includes:
- Raspberry Pi 4



## Installation and configuration

    git clone https://github.com/caseywdunn/tensorflow_lite_pi.git
    cd tensorflow_lite_pi/
    python3 -m venv tf-env
    source tf-env/bin/activate
    bash get_pi_requirements.sh
    wget https://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip
    unzip coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip -d Sample_TFLite_model

## Running
    python3 TFLite_detection_webcam.py --modeldir=Sample_TFLite_model
