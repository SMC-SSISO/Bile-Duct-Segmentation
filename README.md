# Descriptions

- This model is a segmentation model designed to segment the bile duct in Pure Laparoscopic Donor Hepatectomy (PLDH) for Living Donor Liver Transplantation (LDLT). It can help with the anatomical understanding of the biliary structure.
- The model is constructed using the DeepLabV3+ architecture with ResNet50 as an encoder. It was trained with 5-fold cross-validation on 300 images extracted from surgery videos of 30 patients who underwent PLDH surgery.

## Usage

- You can reproduce this model using jupyter notebook we provided.
- You just need to modify the `model_path` and `video_path` within the `inference.ipynb` file.
- You can also download the model weights and a sample video from the link below.
    - https://1drv.ms/f/c/9db2e01a687d3baf/Eg-0KAOhkxxPl5UBGBRjX7ABuhzL9Zm6A7uwc5zZfEgPdg?e=0vYW67

## Preview

**Original video**

![test_video.gif](https://github.com/SMC-SSISO/Bile-Duct-Segmentation/blob/main/gifs/test_video.gif)
                
**Inferenced video**

![inferenced_test_video.gif](https://github.com/SMC-SSISO/Bile-Duct-Segmentation/blob/main/gifs/inferenced_test_video.gif)
                             
## Requiremenets

pytorch==2.2.1

opencv==4.6.0

albumentations==1.3.1

segmentation-models-pytorch==0.3.1

numpy==1.26.4