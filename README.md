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

## Camera.

You can connect a camera to the given C++ examples. With Buster, it was simple. You replaced the filename with a zero (0) and got the images from the RaspiCam instead of a file. Those days are gone with the introduction of Bullseye.

You can use G

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

