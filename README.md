# NC_GAN_Model_for_Covid_Diagnosis

> A GAN Model for Covid Diagnosis Based on Lung CT Images

### Dataset Links

- [echonet-dynamic-cardiac-ultrasound_(not_used)](https://aimi.stanford.edu/echonet-dynamic-cardiac-ultrasound)
- [covid19-image-dataset_(currently_used)](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset)
- [covid19-ct-scans_(not_used)](https://www.kaggle.com/datasets/andrewmvd/covid19-ct-scans)

### Configuration 1/2

- For `AlexNet`, `MLP`, `VGG16`, `VGG19`, `ResNet101V2`, `ResNet152V2`, `EfficientNetB7`, `EfficientV2L`
- `conda env create -f environment_tf.yml`
- Alternative:
```
$ conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
$ python -m pip install tensorflow==2.8.0
$ python -m pip install matplotlib==3.5.2 numpy==1.22.4 pandas==1.4.2 pillow==9.1.1 pip==22.1 requests==2.27.1 scikit-learn==1.1.1 scipy==1.8.1 seaborn==0.11.2 tensorboard==2.8.0 tqdm==4.64.0
```

### Configuration 2/2

- For `ClassicAUG`, `ACGAN_AUG`
- `conda env create -f environment_torch.yml`

### Classic Augmentation

![tran](https://user-images.githubusercontent.com/67775090/170679359-47b4893b-e1df-4de4-aeaa-190fed69629f.png)
