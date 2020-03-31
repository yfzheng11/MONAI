### 1. Requirements
Most of the examples and tutorials require
[matplotlib](https://matplotlib.org/) and [Jupyter Notebook](https://jupyter.org/).

These could be installed by:
```bash
python -m pip install -U pip
python -m pip install -U matplotlib
python -m pip install -U notebook
```

### 2. List of examples
#### [classification_3d](./classification_3d)
Training and evaluation examples of 3D classification based on DenseNet3D and [IXI dataset](https://brain-development.org/ixi-dataset):
The examples are standard PyTorch programs and have both dictionary-based and array-based transformation versions.
#### [classification_3d_ignite](./classification_3d_ignite)
Training and evaluation examples of 3D classification based on DenseNet3D and [IXI dataset](https://brain-development.org/ixi-dataset):
The examples are PyTorch ignite programs and have both dictionary-based and array-based transformation versions.
#### [notebooks/multi_gpu_test](./notebooks/multi_gpu_test.ipynb)
This notebook is a quick demo for devices, run the Ignite trainer engine on CPU, GPU and multiple GPUs.
#### [notebooks/nifti_read_example](./notebooks/nifti_read_example.ipynb)
Illustrate reading NIfTI files and iterating over image patches of the volumes loaded from them.
#### [notebooks/spleen_segmentation_3d](./notebooks/spleen_segmentation_3d.ipynb)
This notebook is an end-to-end training and evaluation example of 3D segmentation based on [MSD Spleen dataset](http://medicaldecathlon.com):
The example shows the flexibility of MONAI modules in a PyTorch-based program:
- Transforms for dictionary-based training data structure.
- Load NIfTI images with metadata.
- Scale medical image intensity with expected range.
- Crop out a batch of balanced image patch samples based on positive / negative label ratio.
- 3D UNet, Dice loss function, Mean Dice metric for 3D segmentation task.
- Sliding window inference.
- Deterministic training for reproducibility.
#### [notebooks/transform_speed](./notebooks/transform_speed.ipynb)
Illustrate reading NIfTI files and test speed of different transforms on different devices.
#### [notebooks/transforms_demo_2d](./notebooks/transforms_demo_2d.ipynb)
This notebook demonstrates the image transformations on histology images using
[the GlaS Contest dataset](https://warwick.ac.uk/fac/sci/dcs/research/tia/glascontest/download/).
#### [notebooks/3d_image_transforms](./notebooks/3D_image_transforms.ipynb)
This notebook demonstrates the transformations on volumetric images.
#### [notebooks/unet_segmentation_3d_ignite](./notebooks/unet_segmentation_3d_ignite.ipynb)
This notebook is an end-to-end training & evaluation example of 3D segmentation based on synthetic dataset.
The example is a PyTorch Ignite program and shows several key features of MONAI,
especially with medical domain specific transforms and event handlers.
#### [segmentation_3d](./examples/segmentation_3d)
Training and evaluation examples of 3D segmentation based on UNet3D and synthetic dataset.
The examples are standard PyTorch programs and have both dictionary-based and array-based versions.
#### [segmentation_3d_ignite](./examples/segmentation_3d_ignite)
Training and evaluation examples of 3D segmentation based on UNet3D and synthetic dataset.
The examples are PyTorch Ignite programs and have both dictionary-base and array-based transformations.