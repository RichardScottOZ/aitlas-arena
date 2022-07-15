

![logo](media/AiTALS_EOBench.png)

# AiTLAS: Benchmark Arena


*AiTLAS: Benchmark Arena* is an open-source benchmark framework for evaluating state-of-the-art deep learning approaches on Earth Observation (EO) image classification tasks. To this end, we present extensive comparative analyses of more than 400 models that stem from nine different state-of-the-art architectures, comparing them on a variety of multi-class and multi-label classification tasks from 22 datasets with different sizes and properties. We benchmark models trained from scratch as well as in the context of transfer learning, leveraging pre-trained model variants, as it is typically performed in practice. All of the presented approaches are general and readily extendable to many other remote-sensing image classification tasks, not included in this study. To ensure reproducibility as well as to facilitate better usability and further developments, here we provide **all experimental details** including the trained models, model configuration and other dataset details used for for this study.

*AiTLAS: Benchmark Arena* is part of the [**AiTLAS**](https://github.com/biasvariancelabs/aitlas) ecosystem, an open-source library for exploratory and predictive analysis of satellite imaginary pertaining to different remote-sensing tasks. 

# Datasets
### Multi-class datasets
|Dataset| Data source | Data Splits |||
|---|---|---|---|---|
|EuroSAT | [github](https://github.com/phelber/EuroSAT) | <a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/eurosat_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/eurosat_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/eurosat_test.csv">test</a>|
|UC Merced| [url](http://weegee.vision.ucmerced.edu/datasets/landuse.html) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/ucmerced_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/ucmerced_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/ucmerced_test.csv">test</a>|
|RSSCN7| [figshare](https://figshare.com/articles/dataset/RSSCN7_Image_dataset/7006946) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsscn7_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsscn7_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsscn7_test.csv">test</a>|
|WHU-RS19| [zip](http://captain.whu.edu.cn/datasets/WHU-RS19.zip) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/whurs19_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/whurs19_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/whurs19_test.csv">test</a>|
|AID| [baidu](https://pan.baidu.com/s/1mifOBv6#list/path=%2F) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/aid_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/aid_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/aid_test.csv">test</a>|
|SIRI-WHU| [figshare](https://figshare.com/articles/dataset/SIRI_WHU_Dataset/8796980) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/siriwhu_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/siriwhu_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/siriwhu_test.csv">test</a>|
|RSI-CB256| [one drive](https://onedrive.live.com/?cid=010149152ff2b56d&id=10149152FF2B56D%21105&authkey=!ADyXDc-zA56zPv4) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsicb256_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsicb256_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsicb256_test.csv">test</a>|
|RESISC45| [one drive](https://onedrive.live.com/?authkey=%21AHHNaHIlzp%5FIXjs&cid=5C5E061130630A68&id=5C5E061130630A68%21107&parId=5C5E061130630A68%21112&action=locate) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/resisc45_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/resisc45_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/resisc45_test.csv">test</a>|
|PatternNet| [gdrive](https://drive.google.com/file/d/127lxXYqzO6Bd0yZhvEbgIfz95HaEnr9K/view) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/patternnet_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/patternnet_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/patternnet_test.csv">test</a>|
|CLRS| [baidu](https://pan.baidu.com/share/init?surl=Xnw9k20Df_ICmkXdvasVqg) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/clrs_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/clrs_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/clrs_test.csv">test</a>|
|RSD46-WHU| [baidu](https://pan.baidu.com/s/1mMDKUu02V0s8rXstewv26A) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsd46whu_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsd46whu_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/rsd46whu_test.csv">test</a>|
|SAT6| [gdrive](https://drive.google.com/uc?id=0B0Fef71_vt3PUkZ4YVZ5WWNvZWs&export=download) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/sat6_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/sat6_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/sat6_test.csv">test</a>|
|Optimal31| [gdrive](https://drive.google.com/file/d/1Fk9a0DW8UyyQsR8dP2Qdakmr69NVBhq9/view) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/optimal31_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/optimal31_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/optimal31_test.csv">test</a>|
|Brazilian Coffee Scenes| [zip](http://www.patreo.dcc.ufmg.br/wp-content/uploads/2017/11/brazilian_coffee_dataset.zip) |<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bcs_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bcs_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bcs_test.csv">test</a>|
|So2Sat| [url](http://doi.org/10.14459/2018MP1454690) |<a href="https://dataserv.ub.tum.de/s/m1483140/download?path=%2F&files=training.h5">train</a>|<a href="https://dataserv.ub.tum.de/s/m1483140/download?path=%2F&files=validation.h5">validation</a>|<a href="https://dataserv.ub.tum.de/s/m1483140/download?path=%2F&files=testing.h5">test</a>|

###  Multi-label datasets

|Dataset| Data source | Data Splits |||
|---|---|---|---|---|
|UC Merced (mlc)|[gdrive](https://drive.google.com/file/d/1DtKiauowCB0ykjFe8v0OVvT76rEfOk0v/view)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/ucmercedmultilabel_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/ucmercedmultilabel_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/ucmercedmultilabel_test.csv">test</a>|
|AID (mlc)|[github](https://github.com/Hua-YS/AID-Multilabel-Dataset)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/aidmultilabel_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/aidmultilabel_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/aidmultilabel_test.csv">test</a>|
|DFC15|[gdrive](https://drive.google.com/drive/folders/1TKGS6TIRxQ6a7gdaj0cHs-mRCtv_J1HA)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/dfc15_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/dfc15_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/dfc15_test.csv">test</a>|
|Planet UAS|[kaggle](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space/overview)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/planetuas_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/planetuas_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/planetuas_test.csv">test</a>|
|MLRSNet|[mendeley](https://data.mendeley.com/datasets/7j9bv9vwsx/2)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/mlrsnet_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/mlrsnet_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/mlrsnet_test.csv">test</a>|
|BigEarthNet 19|[url](http://bigearth.net/)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bigearthnet_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bigearthnet_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bigearthnet_test.csv">test</a>|
|BigEarthNet 43|[url](http://bigearth.net/)|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bigearthnet_train.csv">train</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bigearthnet_val.csv">validation</a>|<a href="https://github.com/biasvariancelabs/LULC/blob/main/splits/bigearthnet_test.csv">test</a>|



# Models

Available **[here](https://drive.google.com/drive/folders/1lTnPsMyyLv9XoPu3cMmE_h6NPkj_WCH8?usp=sharing)**

### Multi-class classification tasks

| Dataset        | Model          | from scratch         | pretrained [ImageNet1K] |
|----------------|----------------|----------------------|-------------------------|
| AID            | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| BCS            | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| CLRS           | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| Eurosat        | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| Optimal31      | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| PatternNet     | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| RESISC45       | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| RSD46-WHU      | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| RSI-CB256      | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| RSSCN7         | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| SAT6           | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| SIRI-WHU       | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| So2Sat         | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| UCMerced       | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| WHU-RS19       | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |



### Multi-label classification tasks

| Dataset        | Model          | from scratch         | pretrained [ImageNet1K] |
|----------------|----------------|----------------------|-------------------------|
| AID (mlc)      | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| BigEarthNet19  | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| BigEarthNet43  | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| DFC15          | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| MLRSNet        | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| PlanetUAS      | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
| UCMerced (mlc) | AlexNet        | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | VGG16          | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet50       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ResNet152      | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | DenseNet161    | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | EfficientNetB0 | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ViT            | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | MLPMixer       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
|                | ConvNeXt       | :heavy\_check\_mark: | :heavy\_check\_mark:    |
