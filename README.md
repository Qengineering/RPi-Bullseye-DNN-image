# Raspberry Pi 4 Bullseye DNN image
![output image]( https://qengineering.eu/images/Water7.webp )<br/>
## A Raspberry Pi 4 Bullseye 64-OS image with deep learning examples
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
## 👉 Bullseye
The [**'old' Buster OS**](https://github.com/Qengineering/RPi-image) is still available.<br><br>
Regularly, we get the question if we have an image of our Raspberry Pi with some frameworks and [our deep-learning examples](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html). We are happy to comply with this request.

------------

## Installation.

- Get a 32 GB SD-card which will hold the image. 
- Download the image Rpi_Bullseye_64_DNN.xz (**4 GByte !**) from [Sync](https://ln5.sync.com/dl/4083226a0/e7t6w7jp-x4vqthff-8v9fxzuh-9y84f2x4).
- Flash the image on the SD-card with the [Imager](https://www.raspberrypi.org/software/) or [balenaEtcher](https://www.balena.io/etcher/).
- Insert the SD-card in your Raspberry Pi 4.
- Wait a few minutes, while the image will expand to the full size of your SD card.
- No WiFi installed. Password: ***3.14***

------------

## Tips.

* Default, the Raspberry Pi is been overclocked to 1850 MHz. See [overclock the Raspberry Pi](https://qengineering.eu/overclocking-the-raspberry-pi-4.html) for more information.<br/>
* If you are in need of extra space, you can delete the opencv and the opencv_contrib folder from the SD-card. There are no longer needed since all libraries are placed in the /usr/local directory.

------------

## Contents.

- [OpenCV](https://github.com/Qengineering/OpenCV-Livecam-Raspberry-Pi)
- [Classification](https://github.com/Qengineering/TensorFlow_Lite_Classification_RPi_64-bits)
- [SSD](https://github.com/Qengineering/TensorFlow_Lite_SSD_RPi_64-bits)
- [Segmentation](https://github.com/Qengineering/TensorFlow_Lite_Segmentation_RPi_64-bit)
- [Segmentation YoloV5](https://github.com/Qengineering/YoloV5-segmentation-ncnn-RPi4)
- [Pose](https://github.com/Qengineering/TensorFlow_Lite_Pose_RPi_64-bits)
- [Face detection](https://github.com/Qengineering/Face-detection-Raspberry-Pi-32-64-bits)
- [Face recognition](https://github.com/Qengineering/Face-Recognition-Raspberry-Pi-64-bits)
- [YoloV5](https://github.com/Qengineering/YoloV5-ncnn-Raspberry-Pi-4)
- [YoloX](https://github.com/Qengineering/YoloX-ncnn-Raspberry-Pi-4)
- [PaddleOCR](https://github.com/Qengineering/PaddleOCR-Lite-Document)
- [Background substraction](https://github.com/Qengineering/Fast-Background-Substraction)
- [Libcamera](https://github.com/Qengineering/Libcamera-OpenCV-RPi-Bullseye-64OS)
- [LVVC](https://github.com/Qengineering/LCCV)

![image](https://github.com/Qengineering/RPi-Bullseye-DNN-image/assets/44409029/3eca9041-9f30-42d5-bed5-f3b0ddfb0726)

------------

## Pre-installed frameworks.

- [OpenCV](https://qengineering.eu/deep-learning-with-opencv-on-raspberry-pi-4.html) 4.7.0
- [TensorFLow](https://qengineering.eu/install-tensorflow-2.4.0-on-raspberry-64-os.html) 2.10.0
- [TensorFlow-Lite](https://qengineering.eu/install-tensorflow-2-lite-on-raspberry-64-os.html) 2.10.0
- [TensorFlow-Lite-Python](https://qengineering.eu/install-tensorflow-2-lite-on-raspberry-64-os.html) 2.10.0
- [Pytorch](https://qengineering.eu/install-pytorch-on-raspberry-pi-4.html) 1.13.0
- [TorchVision](https://qengineering.eu/install-pytorch-on-raspberry-pi-4.html) 0.14.0
- [ncnn](https://qengineering.eu/install-ncnn-on-raspberry-pi-4.html) 20230517
- [MNN](https://qengineering.eu/install-mnn-on-raspberry-pi-4.html) 2.5.0
- [Paddle](https://qengineering.eu/install-paddlepaddle-on-raspberry-pi-4.html) 2.4.2
- [Paddle-Lite](https://qengineering.eu/install-paddle-lite-on-raspberry-pi-4.html) 2.12

![image](https://github.com/Qengineering/RPi-Bullseye-DNN-image/assets/44409029/d4cff548-a053-435c-8926-0f678292c337)

------------

## Camera.

You can connect a camera to the given C++ examples. With Buster, it was simple. You replaced the filename with a zero (0) and got the images from the RaspiCam instead of a file. Those days are gone with the introduction of Bullseye.<br>
Nowadays you have two options. You can either use Gstreamer or LVVC. An example of both can be found in this SD image.
You can also find both methods implemented in the YoloX example.

![image](https://github.com/Qengineering/RPi-Bullseye-DNN-image/assets/44409029/e203e5a1-ea5e-41f7-9e10-2f64f4f511ed)

------------

## WiFi.

Since everyone has a unique password on their WiFi connection, we have not activated the WiFi.<br/>
To enable the wireless LAN follow the next steps:<br/>

1) Left click on the Ethernet symbol.<br/><br/>
![image](https://user-images.githubusercontent.com/44409029/124445112-8eb8e880-dd7f-11eb-80e6-121dc31fd0b8.png)<br/><br/>
2) Click "Turn on wireless LAN", and wait a few seconds. Your RPi will scan for available networks.<br/><br/>
![image](https://user-images.githubusercontent.com/44409029/124445876-39310b80-dd80-11eb-97ff-1ef8f8c477e8.png)<br/><br/>
3) Left click again on the Ethernet symbol and choose your network.<br/><br/>
![image](https://user-images.githubusercontent.com/44409029/124446101-64b3f600-dd80-11eb-9385-eee4fd730268.png)<br/><br/>
4) Give your key, and wait a couple of seconds to let the RPi establish the connection.<br/><br/>
![image](https://user-images.githubusercontent.com/44409029/124447227-74800a00-dd81-11eb-9c47-bee6b2b84bc1.png)<br/><br/>
5) Success! <br/><br/>
![image](https://user-images.githubusercontent.com/44409029/124446775-063b4780-dd81-11eb-9fd8-2d597ad31cee.png)

------------

## TensorFlow-Lite.

Tensorflow-Lite is aimed at small, lightweight devices, such as the Raspberry Pi. Hence the use of a single C++ library.<br>
Since version 2.7, the Tensorflow team has decided to focus on Python for its Lite version. The single large C++ library has since expired.<br>
Now you only have small separate libraries. When programming you will have to specify all the necessary files separately. And these are quite a few.
To make working with Tensorflow-Lite easier, we have packed everything in one package.<br>

![image](https://github.com/Qengineering/RPi-Bullseye-DNN-image/assets/44409029/2eb572c1-a4ab-486d-8045-d7bcb6e24aa0)<br><br>
In addition, it is now also possible to use Tensorflow-Lite in Python.<br>
![image](https://github.com/Qengineering/RPi-Bullseye-DNN-image/assets/44409029/80b81693-6d73-4aa1-9c50-e81d20926a75)<br>
```python
from tflite_runtime.interpreter import Interpreter 
from PIL import Image
import numpy as np
import time

def load_labels(path): # Read the labels from the text file as a Python list.
  with open(path, 'r') as f:
    return [line.strip() for i, line in enumerate(f.readlines())]

def set_input_tensor(interpreter, image):
  tensor_index = interpreter.get_input_details()[0]['index']
  input_tensor = interpreter.tensor(tensor_index)()[0]
  input_tensor[:, :] = image

def classify_image(interpreter, image, top_k=1):
  set_input_tensor(interpreter, image)

  interpreter.invoke()
  output_details = interpreter.get_output_details()[0]
  output = np.squeeze(interpreter.get_tensor(output_details['index']))

  scale, zero_point = output_details['quantization']
  output = scale * (output - zero_point)

  ordered = np.argpartition(-output, 1)
  return [(i, output[i]) for i in ordered[:top_k]][0]

data_folder = "/home/pi/software/TensorFlow_Lite_Classification_RPi_64-bits/"

model_path = data_folder + "mobilenet_v1_1.0_224_quant.tflite"
label_path = data_folder + "labels.txt"

interpreter = Interpreter(model_path)
print("Model Loaded Successfully.")

interpreter.allocate_tensors()
_, height, width, _ = interpreter.get_input_details()[0]['shape']
print("Image Shape (", width, ",", height, ")")

# Load an image to be classified.
image = Image.open(data_folder + "tabby.jpeg").convert('RGB').resize((width, height))

# Classify the image.
time1 = time.time()
label_id, prob = classify_image(interpreter, image)
time2 = time.time()
classification_time = np.round(time2-time1, 3)
print("Classificaiton Time =", classification_time, "seconds.")

# Read class labels.
labels = load_labels(label_path)

# Return the classification label of the image.
classification_label = labels[label_id]
print("Image Label is :", classification_label, ", with Accuracy :", np.round(prob*100, 2), "%.")
```




------------

## OpenCV + TensorFlow.

Importing both TensorFlow and OpenCV in Python can throw the error: _cannot allocate memory in static TLS block_.<br/>
This behaviour only occurs on an aarch64 system and is caused by the OpenMP memory requirements not being met.<br/>
For more information, see GitHub ticket [#14884](https://github.com/opencv/opencv/issues/14884).<br/>

![output image](https://qengineering.eu/images/SwapImportOpenCVRPi.png)

There are a few solutions. The easiest is to import OpenCV at the beginning, as shown above.<br/>
The other is disabling OpenMP by setting the -DBUILD_OPENMP and -DWITH_OPENMP flags OFF.<br/>
Where possible, OpenCV will now use the default pthread or the TBB engine for parallelization.<br/>
We don't recommend it. Not all OpenCV algorithms automatically switch to pthread.<br/>
Our advice is to import OpenCV into Python first before anything else.<br/>

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 

