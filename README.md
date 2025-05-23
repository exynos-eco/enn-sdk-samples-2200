# ENN SDK Samples 2200

## Introduction
|Sample Name|Description|
|-------------|-------|
|[Image Classification In Android](#image-classification-in-android)| Sample Android application to demonstrate the execution of `Inception v4` model with ENN SDK|
|[Object Detection In Android](#object-detection-in-android)| Sample Android application to demonstrate the execution of `YOLOv5` model with ENN SDK|
|[Semantic Segmentation In Android](#semantic-segmentation-in-android)| Sample Android application to demonstrate the execution of `DeeplabV3` model with ENN SDK|
|[Pose Estimation In Android](#pose-estimation-in-android)| Sample Android application to demonstrate the execution of `PoseNet` model with ENN SDK|
|[Image Enhancement In Android](#image-enhancement-in-android)| Sample Android application to demonstrate the execution of `Zero-DCE` model with ENN SDK|
|[Depth Estimation In Andriod](#depth-estimation-in-andriod)| Sample Android application to demonstrate the execution of `MiDaS v2` model with ENN SDK|

## Android (Kotlin) Samples
This section provides an overview of Android (Kotlin) sample applications.
Each sample application entry provides the details of the functionality of the sample application, its location, and instructions for running it.

***

### Image Classification In Android
This sample application demonstrates the execution of a converted [Inception v4](https://www.kaggle.com/models/tensorflow/inception/frameworks/tfLite/variations/v4-quant/versions/1) model using the ENN framework.
The model is converted using ENN SDK service with the **Accelerate** hardware type option.

#### Functionality
The sample application accepts input from a camera feed or an image file and classifies the object within the input.
The classified items, their corresponding scores, and the inference time are displayed at the bottom of the application interface.

#### Location
The sample is available in the `enn-sdk-samples-2200/image-classification` directory within the [Github](https://github.com/exynos-eco/enn-sdk-samples-2200) repository.

#### Getting Started
To utilize the sample application:
1.	Download or clone the sample application from this repository.
2.	Open the sample application project in Android Studio.
3.	Connect the ERD board to the computer.
4.	Run the application (using Shift + F10).
5.	Select Camera or Image mode and provide the data for inference.

To modify the model used in the sample application:
1.	Copy the desired model file to the `assets` directory of the project.
2.	Copy the corresponding label text file to the `assets` directory.
3.	Modify the parameters in the ModelConstants.kt file to reflect the specifications of the new model.
4.	If the inputs and outputs of the model differ from the pre-designed sample application, modify the `preProcess()` and `postProcess()` functions.

***

### Object Detection In Android
This sample application demonstrates the execution of a converted [YOLOv5](https://github.com/ultralytics/yolov5) model using the ENN framework.
The model is converted using ENN SDK service with the **Default** hardware type option.

#### Functionality
The application accepts input from a camera feed or an image file and identifies the object within the input.
A bounding box is drawn around the detected item, and the label and score that are associated with the object are displayed.
Additionally, the inference time is displayed at the bottom of the application interface.

#### Location
The sample is available in the `enn-sdk-samples-2200/object-detection` directory within the [Github](https://github.com/exynos-eco/enn-sdk-samples-2200) repository.

#### Getting Started
To utilize the sample application:
1.	Download or clone the sample application from this repository.
2.	Open the sample application project in Android Studio.
3.	Connect the ERD board to the computer.
4.	Run the application (using Shift + F10).
5.	Select Camera or Image mode and provide the data for inference.

To modify the model used in the sample application:
1.	Copy the desired model file to the `assets` directory of the project.
2.	Copy the corresponding label text file to the `assets` directory.
3.	Modify the parameters in the ModelConstants.kt file to reflect the specifications of the new model.
4.	If the inputs and outputs of the model differ from the pre-designed sample application, modify the `preProcess()` and `postProcess()` functions.

***

### Semantic Segmentation In Android
This sample application demonstrates the execution of a converted [DeeplabV3](https://www.kaggle.com/models/tensorflow/deeplabv3/frameworks/tfLite/variations/default/versions/1) model using the ENN framework.
The model is converted using ENN SDK service with the **Default** hardware type option.

#### Functionality
The application accepts input from a camera feed or an image file and segmentation objects within the input.
Each pixel of the segmented object is overlayed with a color corresponding to its label, thereby providing a visual representation of the classification.
Additionally, the inference time is displayed at the bottom of the application interface.

#### Location
The sample is available in the `enn-sdk-samples-2200/semantic-segmentation` directory within the [Github](https://github.com/exynos-eco/enn-sdk-samples-2200) repository.

#### Getting Started
To utilize the sample application:
1.	Download or clone the sample application from this repository.
2.	Open the sample application project in Android Studio.
3.	Connect the ERD board to the computer.
4.	Run the application (using Shift + F10).
5.	Select Camera or Image mode and provide the data for inference.

To modify the model used in the sample application:
1.	Copy the desired model file to the `assets` directory of the project.
2.	Modify the parameters in the ModelConstants.kt file to reflect the specifications of the new model.
3.	If the inputs and outputs of the model differ from the pre-designed sample application, modify the `preProcess()` and `postProcess()` functions.

***

### Pose Estimation In Android
This sample application demonstrates the execution of a converted [PoseNet](https://www.kaggle.com/models/tensorflow/posenet-mobilenet/frameworks/tfJs/variations/float-075/versions/1) model using the ENN framework.
The model is converted using ENN SDK service with the **Default** hardware type option.

#### Functionality
The application accepts input from a camera feed or an image file.
Then, it detects the points of a person and overlays the points and edges of a person.
Additionally, the inference time is displayed at the bottom of the application interface.

#### Location
The sample is available in the `enn-sdk-samples-2200/pose-estimation` directory within the [Github](https://github.com/exynos-eco/enn-sdk-samples-2200) repository.

#### Getting Started
To utilize the sample application:
1.	Download or clone the sample application from this repository.
2.	Open the sample application project in Android Studio.
3.	Connect the ERD board to the computer.
4.	Run the application (using Shift + F10).
5.	Select Camera or Image mode and provide the data for inference.

To modify the model used in the sample application:
1.	Copy the desired model file to the `assets` directory within the project.
2.	Modify the parameters in the ModelConstants.kt file to reflect the specifications of the new model.
3.	If the inputs and outputs of the model differ from the pre-designed sample application, modify the `preProcess()` and `postProcess()` functions.

***

### Image Enhancement In Android
This sample application demonstrates the execution of a converted [Zero-DCE](https://www.kaggle.com/models/sayannath235/zero-dce) model using the ENN framework.
The model is converted using ENN SDK service with the **Default** hardware type option.

#### Functionality
The application accepts input from an image file and enhances it.
Specifically, it takes low-light images and improves their quality.
Additionally, the inference time is displayed at the bottom of the application interface.

#### Location
The sample is available in the `enn-sdk-samples-2200/image-enhancement` directory within the [Github](https://github.com/exynos-eco/enn-sdk-samples-2200) repository.

#### Getting Started
To utilize the sample application:
1.	Download or clone the sample application from this repository.
2.	Open the sample application project in Android Studio.
3.	Connect the ERD board to the computer.
4.	Run the application (using Shift + F10).
5.	Provide the image data for inference.

To modify the model used in the sample application:
1.	Copy the desired model file to the `assets` directory of the project.
2.	Modify the parameters in the ModelConstants.kt file to reflect the specifications of the new model.
3.	If the inputs and outputs of the model differ from the pre-designed sample application, modify the `preProcess()` and `postProcess()` functions.

***

### Depth Estimation In Andriod
This sample application demonstrates the execution of a converted [MiDaS V2](https://www.kaggle.com/models/intel/midas/frameworks/tfLite/variations/v2-1-small-lite/versions/1) model using the ENN framework.
The model is converted using ENN SDK service with the **Default** hardware type option.

#### Functionality
The application accepts input from a camera feed or an image file.
A color that represents the estimated distance is overlayed on each pixel, thereby providing a visual representation of depth.
Additionally, the inference time is displayed at the bottom of the application interface.

#### Location
The sample is available in the `enn-sdk-samples-2200/depth-estimation` directory within the [Github](https://github.com/exynos-eco/enn-sdk-samples-2200) repository.

#### Getting Started
To utilize the sample application:
1.	Download or clone the sample application from this repository.
2.	Open the sample application project in Android Studio.
3.	Connect the ERD board to the computer.
4.	Run the application (using Shift + F10).
5.	Select Camera or Image mode and provide the data for inference.

To modify the model used in the sample application:
1.	Copy the desired model file to the `assets` directory of the project.
2.	Modify the parameters in the ModelConstants.kt file to reflect the specifications of the new model.
3.	If the inputs and outputs of the model differ from the pre-designed sample application, modify the `preProcess()` and `postProcess()` functions.

***

## Native Samples
This section provides an overview of the native sample program.
Each sample program entry provides the functionality of the sample program, its location, and instructions for running it.

***