## Classic Augmentation Based Classifier Generative Adversarial Network (CACGAN) for COVID-19 Diagnosis

- Trained the Generator with a custom loss function to enable it to generate new data in specific classes
- Trained the Discriminator with the original data set and the data generated by the Generator
- Evaluated the performance of the GAN model by multiple classifiers (VGG, ResNet, EfficientNet, etc.)

### Dataset Links

- [covid19-image-dataset](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset)

### Configuration

- `conda env create -f environment_dl.yml`
- **`environment_dl.yml` may contains some packages that won't be used here! If you are disk-sensitive, please only install the packages appeared in scripts :)**

### Usage

- `ClassicHistEqual.ipynb` for histogram equalization and `ClassicAUG.ipynb` for classic augmentation
- `CACGAN_AUG.ipynb` for data synthetizing using an AC-GAN model
- `GenerateData.ipynb` for generating new data to `./GANGEN` through the Generator saved during training
- folders `[augmented, original, synthetic]` are results of multiple classifiers on augmented data, original data, and synthetic data, respectively

### Classic Augmentation

![tran](https://user-images.githubusercontent.com/67775090/170679359-47b4893b-e1df-4de4-aeaa-190fed69629f.png)

### Histogram Equalization

<img src="https://user-images.githubusercontent.com/67775090/187150691-c1474cf2-2617-4166-9d42-41d3fe404193.png" width="540px">

### Lung CT Images Generated by the Generator After 1, 20, 50, 100, 500, 1000 Epochs

![image](https://user-images.githubusercontent.com/67775090/187150340-d5c884e5-eefb-4c65-8644-7f490b2bb949.png)

### Generated Data of the Generator After the Last Iteration (Left), and the Real Data (Right)

![image](https://user-images.githubusercontent.com/67775090/187150465-f786af59-d861-49e9-95b5-76b5fa992592.png)

### Structure of Generator and Discriminator

![image](https://user-images.githubusercontent.com/67775090/187150911-912a6284-287d-4a21-a857-4ea37dd81738.png)

### Training Process

![image](https://user-images.githubusercontent.com/67775090/187151209-8b570753-fce0-4edb-8d4c-87f3fb729561.png)

