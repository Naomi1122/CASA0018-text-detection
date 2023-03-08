# CASA0018
## Project Idea

The project aim is to build a text detection system to extract text from real-world images, can be devided into 2 steps:
1. text detection, use segmentation techniques
2. text recognition, extract raw text from the cropped part of the input images

Project physical platform: ios iphone

Here is an example to show the process pipeline
![ocr pipeline](https://user-images.githubusercontent.com/78373920/223587531-a6dea7c3-0fdb-41b9-9cf0-9a9bbb33d72a.jpg)

image regions that contains text are cropped -> CNN feature extract -> LSTM -> CTC decoder

CTC is used as it helps to ignore both the position and the width of the symbols in the image, recognized text is not process further.

Dataset:

Synthetic Word Dataset

Example
![data1](https://user-images.githubusercontent.com/78373920/223589146-90fe6af5-7806-43bd-903f-029e9060e7fa.jpg)
![data2](https://user-images.githubusercontent.com/78373920/223589336-01945493-7d3d-4cc6-8933-7a2a0301fbe4.jpg)
