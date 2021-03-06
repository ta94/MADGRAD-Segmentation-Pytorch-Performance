## MADGRAD-Segmentation-Pytorch-Performance
    Compare the performance of MADGRAD against Adam and SGD for segmentation model training.

#### Pascal VOC2012 Segmentation
##### CrossEntropyLoss

<img  src="figures/crossentropyloss_SGD.png" width="35%">
<img  src="figures/crossentropyloss_ADAM.png" width="35%">
<img  src="figures/crossentropyloss_MADGRAD.png" width="35%">

##### Pixel Accuracy

<img  src="figures/pixelaccuracy_SGD.png" width="35%">
<img  src="figures/pixelaccuracy_ADAM.png" width="35%">
<img  src="figures/pixelaccuracy_MADGRAD.png" width="35%">




##### Setup Conda Env
    - conda env create -f env.yml

##### VOC2012 Segmentation Training 

    -  SDG
        ~/anaconda3/envs/pytorch17_102/bin/python train.py SGD
    -  Adam
        ~/anaconda3/envs/pytorch17_102/bin/python train.py Adam
    -  MADGRAD
        ~/anaconda3/envs/pytorch17_102/bin/python train.py MADGRAD

##### References
    - https://github.com/jfzhang95/pytorch-deeplab-xception.git (dataloaders, pascal.py)