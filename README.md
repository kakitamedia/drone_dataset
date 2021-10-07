# Distant Bird Detection Dataset for Safe Drone Flight

In this work, we propose a large dataset of bird detections captured by a drone camera at a large diversity of locations.

<img src='images/samples.png'/>

## Overview
Our dataset 
* contains images with various backgrounds such as in fields, mountains ,and near houses.
* 


## Annotation format

```yaml
[
    {
        'path': file_path,
        'bbox': [
            [x1, y1, w, h],
            [x2, y2, w, h],
        ]
        'label': [
            'hawk',
            'crow',
        ]
    }
    ...
]
```

## Data access

[Images](https://drive.google.com/file/d/10_gyG5GQLNRX89SUuSG1xy8MSUlbNwzv/view?usp=sharing)

[train]() | [val]()

## Citation
If you are using our dataset, please add a reference to our paper.

```
@inproceedings{,
  title={Distant Bird Detection for Safe Drone Flight and Its Dataset},
  author={Sanae, Fujii and Kazutoshi, Akita and Ukita, Norimichi},
  booktitle={International Conference on Machine Vision Applications (MVA)},
  year={2021}
}
```
