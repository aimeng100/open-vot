# Open-VOT

Open-VOT is a lightweight library of visual object tracking for research purpose. It aims to provide a uniform interface for different datasets, a full set of models and evaluation metrics, as well as examples to reproduce (near) state-of-the-art results.

*Currently two trackers are implemented: [SiamFC](http://www.robots.ox.ac.uk/~luca/siamese-fc.html) and [GOTURN](http://davheld.github.io/GOTURN/GOTURN.html). We aim to include more state-of-the-art trackers. Please comment if you have any recommendations.*

## Installation

*Currently only Python3 is supported.*

Install [PyTorch](http://pytorch.org/) (version >= 0.4.0) and other dependencies:

```shell
pip install torchvision opencv-python-contrib h5py scipy matplotlib tensorboardX
```

## Examples

**Tracking with pretrained models**

Download pretrained models from [here](https://pan.baidu.com/s/1OutjOlWxmiiA4qna7UFHGg), then execute the following command:

```shell
python examples/goturn --phase test
```

**Training**

```shell
python examples/siamfc --phase train
```

The command trains SiamFC tracker on the ImageNet VID dataset, which can be found and downloaded at [Kaggle](https://www.kaggle.com/c/imagenet-object-detection-from-video-challenge/data).

Please check out more examples in the `examples` folder. Or, alternatively, you could find out more concise examples in the `tests/trackers` folder.
