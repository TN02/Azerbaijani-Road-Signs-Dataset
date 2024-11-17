# Azerbaijani-Road-Signs-Dataset

The Azerbaijani Road Signs Dataset is a dataset that was assembled by combining various publicly available datasets and adding additional captured images.

Annotations are in Pascal VOC format. Most of the images were labelled manually.

The dataset was used to train an object detection model called "SSD-MobileNet-V2," which was tested on a Jetson Nano. The [guide](https://github.com/dusty-nv/jetson-inference/blob/master/docs/pytorch-ssd.md) by ["dusty-nv"](https://github.com/dusty-nv) was followed for training the model.

## Datasets

1. [GTSRB - German Traffic Sign Recognition](https://benchmark.ini.rub.de/gtsrb_dataset.html)

2. [RTSD - Russian Traffic Sign Dataset](https://graphics.cs.msu.ru/projects/traffic-sign-recognition.html)

3. Additional 230 images taken in different parts of Baku 

P.S. The sourced datasets were taken from "roboflow.ai" website.

## Labels

| Type Of Road Sign    | Number of Images |
| ---------------------| ---------------- |
| UTurn                | 384              |
| Turn Left            | 382              |
| Straight or Left     | 426              |
| Turn Right           | 453              |
| Round Ahead          | 464              |
| No Waiting           | 509              |
| Parking Sign         | 521              |
| Straight or Right    | 600              |
| Pedestrian Crossing  | 672              |
| Speed Warning 90     | 685              |
| Ahead Only           | 1074             |
| Speed Warning 60     | 1410             |
| No Overtaking        | 1719             |
| Speed Warning 70     | 1980             |
| Speed Warning 40     | 2114             |
| STOP                 | 2427             |
| Give Away            | 2440             |
| Main Road            | 2458             |
| No Entry             | 2473             |
| No Parking           | 3607             |

Total: 26978 images 

## Usage

Explanation of each folder and file:

1. *Annotations* - These are annotations (.xml) in Pascal VOC format. The name of the file is the same name as an image file. Inside this file, the annotation describes a labeled object within an image. 

2. *ImageSets* - This folder is for the system to get the names of the files.

3. *JPEGImages* - Images of road signs

4. *labels.txt* - All the labels of the images.

5. *mb2-ssd-lite-mp-0_686.pth* - Trained model. You can use on Jetson for testing purposes.

## Contributing

This project was done in July 2023 by:
1. Nazim Talibzade (LinkedIn: https://www.linkedin.com/in/nazim-talibzade-892945238/ )
2. Nijat Aliyev (LinkedIn: https://www.linkedin.com/in/nijat-aliyev-62b5a627b/ )
3. Orkhan Rafiyev (LinkedIn: https://www.linkedin.com/in/orkhan-rafiyev-496792218/ )
4. Nazrin Khalilova (LinkedIn: https://www.linkedin.com/in/nazrin-aliyeva-frontend/ )

Paper: http://dx.doi.org/10.13140/RG.2.2.33333.90084

## License

[MIT](https://choosealicense.com/licenses/mit/)
