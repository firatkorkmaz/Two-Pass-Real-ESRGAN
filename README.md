# Two-Pass Real-ESRGAN Image Enhancement
A Notebook program written in Google Colab to run 2-pass image enhancement process with Real-ESRGAN.

## General Information
[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) is an image enhancement program that has different models to enhance images with optional increase in image sizes.

This Notebook downloads and uses 3 different models from the original project:

1. [RealESRGAN_x4plus.pth](https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.0/RealESRGAN_x4plus.pth)
2. [RealESRGAN_x4plus_anime_6B.pth](https://github.com/xinntao/Real-ESRGAN/releases/download/v0.2.2.4/RealESRGAN_x4plus_anime_6B.pth)
3. [RealESRNet_x4plus.pth](https://github.com/xinntao/Real-ESRGAN/releases/download/v0.1.1/RealESRNet_x4plus.pth)

There are 2 different prompt types for each model where one is for single-pass enhancement and the other is for two-pass enhancement. Besides the performance difference between the models, it is observed that two-pass process always gives better results than one-pass process for each model and this Notebook is intended to provide the two-pass enhancement prompt examples for the RealESRGAN program. There are 2 Zip files provided in this project:
* **input.zip**: An input image sample given in a zip file to test the program.
* **outputs_x2_x2.zip**: Output of the enhancement implemented on the input file.

**Single-Pass & Two-Pass Enhancement Comparison**
* The first image is the result of Single-Pass ESRGAN enhancement on the input image with 4x rescaling.
* The second image is the result of Two-Pass ESRGAN enhamcement on the input image with 2x & 2x = 4x rescaling.

<img title="Single-Pass Real-ESRGAN" src="https://github.com/firatkorkmaz/Two-Pass-Real-ESRGAN/blob/main/images/input_x4_ganx4.png" height="400"> <img title="Two-Pass Real-ESRGAN" src="https://github.com/firatkorkmaz/Two-Pass-Real-ESRGAN/blob/main/images/input_x2_x2_ganx4_ganx4.png" height="400">

## Setup & Run
* Upload the **Real_ESRGAN.ipynb** file to your Google Drive and open it in Google Colab with GPU runtime type enabled.
* Your input images to be enhanced must be provided in a Zip file when it is asked from one of the Notebook cells.
