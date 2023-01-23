<div align="center">
  <p>
    <a align="center" href="https://ultralytics.com/yolov8" target="_blank">
      <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/banner-yolov8.png"></a>
  </p>

<br>

<div>
    <a href="https://github.com/ultralytics/ultralytics/actions/workflows/ci.yaml"><img src="https://github.com/ultralytics/ultralytics/actions/workflows/ci.yaml/badge.svg" alt="Ultralytics CI"></a>
    <a href="https://zenodo.org/badge/latestdoi/264818686"><img src="https://zenodo.org/badge/264818686.svg" alt="YOLOv8 Citation"></a>
    <a href="https://hub.docker.com/r/ultralytics/ultralytics"><img src="https://img.shields.io/docker/pulls/ultralytics/ultralytics?logo=docker" alt="Docker Pulls"></a>
    <br>
    <a href="https://console.paperspace.com/github/ultralytics/ultralytics"><img src="https://assets.paperspace.io/img/gradient-badge.svg" alt="Run on Gradient"/></a>
    <a href="https://colab.research.google.com/github/ultralytics/ultralytics/blob/main/examples/tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
    <a href="https://www.kaggle.com/ultralytics/yolov8"><img src="https://kaggle.com/static/images/open-in-kaggle.svg" alt="Open In Kaggle"></a>
  </div>
<br>

[Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics), developed by [Ultralytics](https://ultralytics.com),
is a cutting-edge, state-of-the-art (SOTA) model that builds upon the success of previous YOLO versions and introduces
new features and improvements to further boost performance and flexibility. YOLOv8 is designed to be fast, accurate, and
easy to use, making it an excellent choice for a wide range of object detection, image segmentation and image
classification tasks.

<img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/main/yolov8/yolo-comparison-plots.png"></a>
</div>

## Installation

``` shell
# clone repo
git clone https://github.com/akanametov/ultralytics

# pip install required packages
pip install ultralytics

# go to code folder
cd ultralytics
```

</details>

## Inference

On image:

```shell
yolo task=detect \
mode=predict \
model=yolov8m-football.pt \
conf=0.25 \
source=examples/football.jpg
```

<div align="center">
    <a href="./">
        <img src="./results/football.jpg" width="90%"/>
    </a>
</div>

## Results

PR curve:
<div align="center">
    <a href="./">
        <img src="./results/P_curve.png" width="30%"/>
    </a>
    <a href="./">
        <img src="./results/PR_curve.png" width="30%"/>
    </a>
    <a href="./">
        <img src="./results/R_curve.png" width="30%"/>
    </a>
</div>

Losses and mAP:
<div align="center">
    <a href="./">
        <img src="./results/results.png" width="80%"/>
    </a>
</div>

Confusion matrix:
<div align="center">
    <a href="./">
        <img src="./results/confusion_matrix.png" width="70%"/>
    </a>
</div>

## Training

Data preparation

* Download [dataset](https://universe.roboflow.com/roboflow-jvuqo/football-players-detection-3zvbc/dataset/2#):

``` shell
bash scripts/get_dataset.sh
```
and pretrained [yolov8m.pt](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt) model.

Single GPU training

``` shell
# train model
yolo task=detect \
mode=train \
model=yolov8m.pt \
data=datasets/data.yaml \
epochs=100 \
imgsz=640
```

## Transfer learning

[`yolov8m.pt`](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8m.pt)

## <div align="center">License</div>

YOLOv8 is available under two different licenses:

- **GPL-3.0 License**: See [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for details.
- **Enterprise License**: Provides greater flexibility for commercial product development without the open-source
  requirements of GPL-3.0. Typical use cases are embedding Ultralytics software and AI models in commercial products and
  applications. Request an Enterprise License at [Ultralytics Licensing](https://ultralytics.com/license).

## <div align="center">Contact</div>

For YOLOv8 bugs and feature requests please visit [GitHub Issues](https://github.com/ultralytics/ultralytics/issues).
For professional support please [Contact Us](https://ultralytics.com/contact).

<br>
<div align="center">
  <a href="https://github.com/ultralytics" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-github.png" width="3%" alt="" /></a>
  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
  <a href="https://www.linkedin.com/company/ultralytics" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-linkedin.png" width="3%" alt="" /></a>
  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
  <a href="https://twitter.com/ultralytics" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-twitter.png" width="3%" alt="" /></a>
  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
  <a href="https://www.producthunt.com/@glenn_jocher" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-producthunt.png" width="3%" alt="" /></a>
  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
  <a href="https://youtube.com/ultralytics" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-youtube.png" width="3%" alt="" /></a>
  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
  <a href="https://www.facebook.com/ultralytics" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-facebook.png" width="3%" alt="" /></a>
  <img src="https://github.com/ultralytics/assets/raw/main/social/logo-transparent.png" width="3%" alt="" />
  <a href="https://www.instagram.com/ultralytics/" style="text-decoration:none;">
    <img src="https://github.com/ultralytics/assets/raw/main/social/logo-social-instagram.png" width="3%" alt="" /></a>
</div>
