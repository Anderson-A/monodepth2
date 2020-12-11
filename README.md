# Exploring the Transferability of Unupervised Monocular Depth Estimation Networks

**Group Members:** Anderson Adon and Eugene Asare

**Experiments Ran (each are evaluated on a test split NYU Depth 2)**

- Trained on KITTI
- Trained on NYU Depth 2
- Trained on KITTI, Finetuned on NYU Depth 2
- Trained on KITTI, Finetuned on NYU Depth 2 using 7 frames
- Trained on KITTI, FFinetuned on NYU Depth 2 using 7 frames and learning rate of 0.001

**Files Added to MonoDepth2**

- [nyu_dataset.py](https://github.com/Anderson-A/monodepth2/blob/master/datasets/nyu_dataset.py): adds new dataset class for us to use NYU Depth 2
- [splits/nyu/](https://github.com/Anderson-A/monodepth2/tree/master/splits/nyu): train, valid, and test splits of NYU Depth 2 dataset
- [bash_scripts/](https://github.com/Anderson-A/monodepth2/tree/master/bash_scripts): scripts to run experiments listed above

**Files Modified from MonoDepth2**

- [evaluate_depth.py](https://github.com/Anderson-A/monodepth2/blame/master/evaluate_depth.py): added capabilty to evaluate on NYU Depth 2
- [options.py](https://github.com/Anderson-A/monodepth2/blame/master/options.py): added capability to use NYU Depth 2 during training and evaluation
- [trainer.py](https://github.com/Anderson-A/monodepth2/blame/master/trainer.py): added capability to train on NYU Depth 2
