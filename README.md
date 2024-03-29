# Distant Bird Detection Dataset for Safe Drone Flight

In this repository, we provide a dataset of bird detections captured by a drone camera at various locations proposed in our [paper](http://www.mva-org.jp/Proceedings/2021/papers/O1-1-3.pdf?fbclid=IwAR2CwkCVoLEDIfAUxhSzPnA44QYXR5MkJzevGsACb7zFX9hI216z1TinCME).

<img src='images/samples.png'/>

## Abstract

For the safe flight of drones, they must avoid the attacks of aggressive birds. These birds move very fast and must be detected far enough away. In recent years, deep learning has made it possible to detect small distant objects in RGB camera images. Since these methods are learning-based, they require a large amount 
of training images, but there are no publicly-available datasets for bird detection taken from drones. In this work, we propose a new dataset captured by a drone camera in various locations (e.g., fields, mountains, near houses).

## Update
[2023/02/23] Bug fix: Fix some annotation errors </br>
[2023/01/29] Bug fix: Delete duplicate instances in annotation files </br>
[2023/01/18] Split the zip file of images </br>
[2021/10/07] Add extra data (21,837 → 47,260 annotated images)

## Licecnse

Our dataset is released under the [MIT license](https://github.com/kakitamedia/drone_dataset/blob/main/LICENSE).

## Dataset overview
Our dataset 
* contains 60,971 manually annotated bird instances in 47,260 images with a resolution of 3840 × 2160 pixels (~67GB).
* is devided into 42,790 training images with 52,036 instances and 4,470 validation images with 8,935 instances.
* have 3 object labels (i.e., hawk, crow, and wild bird.)

## Annotation format

Our annotation JSON file consists of the following fields.

```yaml
[
    {
        'path': 'path_to_image',
        'bbox': [
            [x1, y1, w1, h1],
            [x2, y2, w2, h2],
            ...
        ]
        'label': [
            'label1',
            'label2',
            ...
        ]
    }
    ...
]
```

## Data access

### [Images](https://drive.google.com/drive/folders/11H30-Oh_Ybi_LzsRot2soHaNp2ZWlt4i?usp=share_link) | [Annotations](https://drive.google.com/file/d/1P-yM34AjsRXFDyOzGW7MbJnpuP3f3IKy/view?usp=share_link)

## Citation
Please cite this [paper](http://www.mva-org.jp/Proceedings/2021/papers/O1-1-3.pdf?fbclid=IwAR2CwkCVoLEDIfAUxhSzPnA44QYXR5MkJzevGsACb7zFX9hI216z1TinCME) in your publications if this dataset helps your research..

```
@inproceedings{,
  title={Distant Bird Detection for Safe Drone Flight and Its Dataset},
  author={Sanae Fujii and Kazutoshi Akita and Norimichi Ukita},
  booktitle={International Conference on Machine Vision Applications (MVA)},
  year={2021}
}
```
