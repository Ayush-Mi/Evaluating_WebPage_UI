# Evaluating_WebPage_UI

## Description
In this project I have explored ways to detect elements in a web page layout. It uses deep learning based object detection methods to detect from a set of eight objects and create bounding boxes around them.

## Application
It could potentially be used to rank web page layouts based upon the quality of information it has like portion of the page covered by advertisements, portion covered by images/texts, ratio of buttons to the whole frame etc.

## Method
To detect and classify elements of web page, deep learning object detection method has been used. I have fine tuned ResNet50 based SSD model which was pretrained on coco dataset and taken from tensorflow-garden.

## Dataset
The dataset was taken from [Roboflow](https://public.roboflow.com/object-detection/website-screenshots)
There were 8 lables in the whole data:
- Button
- Field
- iFrame
- Image
- Heading
- Label
- Link
- Text

Train Data Distribution | Val Data Distribution | Test Data Distribution
:---: | :---: | :---:
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/img/train.png) | ![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/img/val.png) | ![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/img/test.png)

## Training
The entire model was fine tuned for 5 epochs with training loss reaching to 0.59 on Mac M1-pro with 32gb of memory. It took around 45 mins for 1688 images to run single training epoch 

## Results

#### Image 1
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_118.jpg)

#### Image 2
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_119.jpg)

#### Image 3
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_110.jpg)

#### Image 4
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_111.jpg)

#### Image 5
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_112.jpg)

#### Image 6
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_113.jpg)

#### Image 7
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_114.jpg)

#### Image 8
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_115.jpg)

#### Image 9
![](https://github.com/Ayush-Mi/Evaluating_WebPage_UI/blob/main/results/gif_frame_116.jpg)

## Future Works
Limited by the time and resource the model was not optimized to accuracy. By tweaking architecture and running the trainings for more number of epochs, better results can be achieved.

## Acknowledgements
[RoboFlow](https://public.roboflow.com/object-detection/website-screenshots)
