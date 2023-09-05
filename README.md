# Adobe's Entity Segmentation dataset
![image](preview.png)

This repository provides mask annotations and image URLs for the EntitySeg dataset as described in the ICCV2023 paper:

### &emsp; High-Quality Entity Segmentation
&emsp;&nbsp; Lu Qi, Jason Kuen, Tiancheng Shen, Weidong Guo, Jiuxiang Gu, Jiaya Jia, Zhe Lin, Ming-Hsuan Yang.

## Download annotation files
Please refer to `v1.0` release of this repo.

## Annotation format
annotations[{<br />
&emsp;'**area**': int,<br />
&emsp;'**image_id**': int,<br />
&emsp;'**bbox**': [x,y,width,height],<br />
&emsp;'**category_id**': int (class-agnostic),<br />
&emsp;'**segmentation**': dict (mask annotation in pycocotools RLE format),<br />
&emsp;'**id**': int,<br />
&emsp;'**category_id_ori**': str (class-aware),<br />
}]

images[{<br />
&emsp;'**file_name**': str,<br />
&emsp;'**height**': int,<br />
&emsp;'**width**': int,<br />
&emsp;'**id**': int,<br />
&emsp;'**img_source**': str,<br />
&emsp;'**url_flag**': str,<br />
&emsp;'**url_dataset**': str,<br />
&emsp;'**url_image**': str,<br />
}]

## Download images
Images can be downloaded through the image source entries and/or URLs that we provide in the annotation files.

## Citation
Please cite our ICCV2023 paper if you use the EntitySeg dataset in your work.
````
@InProceedings{Qi_2023_EntitySeg,
    author    = {Qi, Lu and Kuen, Jason and Shen, Tiancheng and Gu, Jiuxiang and Guo, Weidong and Li, Wenbo and Jia, Jiaya and Lin, Zhe and Yang, Ming-Hsuan},
    title     = {High-Quality Entity Segmentation},
    booktitle = {International Conference on Computer Vision (ICCV)},
    month     = {October},
    year      = {2023},
}
````

## License
This dataset is released under [Adobe Research License](LICENSE.md). The license prohibits commercial use and allows for non-commercial research use.
