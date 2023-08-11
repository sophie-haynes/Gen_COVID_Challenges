# Generalisable-COVID19

This repository contains all the code, model and data references from our cross-dataset evaluative study of COVID-19 models. 

# Contents
1. [Models](#Models)
2. [Datasets](#Datasets)

## Models
Since most of our models exceed the size limits of GitHub lfs free storage, we have made them available for download [here](https://www.dropbox.com/sh/97ap1u84qqwn2xl/AAAs2e4WaHRbxQFLawH6Q0SVa?dl=0).
- [Conv-4](https://www.dropbox.com/sh/xrgsi0fy5qxnrm0/AACV8Uw8FhHCx65gZkLTsKCHa?dl=0)
- [DenseNet 121 (CXR-8 Pre-trained)](https://www.dropbox.com/sh/br0srv71tm2box9/AAAOFQlEzLO4-a3yC8lNmfoXa?dl=0)
- [DenseNet 121 (ImageNet Pre-trained)](https://www.dropbox.com/sh/7ay5miy1wpqv7wu/AAA-b2kvFz8sx1oC0F5cFb1ga?dl=0)
- [DenseNet 121 (Wehbe Private COVID-19 Data Pre-trained)](https://www.dropbox.com/sh/8ltxmyph0bldmgu/AAAI2k6aMKiPWtpSSjeboLUza?dl=0) *see [Wehbe et al. (2021) "DeepCOVID-XR"](https://pubs.rsna.org/doi/abs/10.1148/radiol.2020203511)*
- [ReseNet 16 (Minaee Deep-COVID)](https://www.dropbox.com/sh/7txl44o2mx3pctl/AAA5FT-tlrkYc6SWQCj4rQboa?dl=0) *see [Minaee et al. (2020) "Deep-COVID"](http://www.pubmedcentral.nih.gov/articlerender.fcgi?artid=PMC7372265)*
- [DarkCovidNet](https://www.dropbox.com/sh/zv9sblzqz6nac90/AAA9JaBRVaCsf5BL8oE9Y8Bga?dl=0)

## Datasets
Due to data regulations, as well as storage limitations, we are unable to directly share the datasets we used for our study. Instead, we provide all non-sensitive data required to reproduce the datasets manually. Note that the [BRAX dataset]([url](https://physionet.org/content/brax/1.1.0/)) used in external dataset I requires obtaining credentialled access before downloading. Please refer to the details on the BRAX website.

### Internal Train & Test
In this study, we use the COVID-19 dataset shared by Minaee et al. (2020), *DeepCovid*. The authors have shared the dataset [here](https://www.dropbox.com/s/9w8nmj791c9ogsx/data_upload_v3.zip?dl=0). We use the same train and test split as the authors.

### External I
This dataset set combines specific newly added COVID-19 images from the Cohen et al. (2020) [**covid-chestxray** dataset](https://github.com/ieee8023/covid-chestxray-dataset) and *no finding* and *pneumonia* images from the [**BRAX** dataset](https://physionet.org/content/brax/1.1.0/). BRAX access requires users to create a Physionet account and to complete the data specimens training. As such, we are unable to share the images directly. Instead, we share a csv which contains the anonymised image names of images used in our study. This includes image names of the COVID samples, which should allow you to filter images to reproduce our test set.

### External II
This dataset can be downloaded from [Kaggle](https://www.kaggle.com/competitions/siim-covid19-detection). To download, you will need to create a Kaggle account, then join the competition. In our study, to speed up data handling, we performed image preprocessing on the Kaggle website and downloaded the smaller PNGs. The notebook is available [here](https://www.kaggle.com/kawaiikeewee/convert-siim-dicom-to-png).

### External III
The data for External III can be downloaded from the Tabik et al. (2020) [**COVIDGR** dataset](https://github.com/ari-dasci/OD-covidgr). 
