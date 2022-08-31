# BME580 Final Project - Hair Removal Segmentation using U-Net

### Abstract 
Skin cancer is the most common type of cancer [1]. Early skin cancer detection is critical for treatment and increasing survival rate. In recent years, deep learning approaches have been used to classify, segment, and detect skin lesions from dermoscopic images. This paper examines how segmentation performance is affected by the image acquisition process from the dermatoscope. The image acquisition process is automated by adding color channels, illumination patterns, and lens blur as physical layers with tunable parameters into U-Net and MultiResUNet deep convolutional neural networks (CNN). The results suggest that the U-Net outperforms MultiResUNet in dermoscopic skin lesion boundary segmentation, with a dice coefficient of 0.7844 and Jaccard index of 0.6784. While optimizing for the physical components in a U-Net did not improve segmentation  performance in terms of dice coefficient and Jaccard index, optimizing for color channels and lens blur did improve performance results for MultiResUNet. These findings can aid researchers in developing an ideal imaging system that is time-efficient, cost-efficient, and accurate for skin cancer detection.

This repo contains: 

* U_Net_Models.ipynb - Code and results

### Built With

* [Google Colab](https://colab.research.google.com/)

### Install

This project requires **Python** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [Tensor Flow](https://www.tensorflow.org/)
- [Keras](https://keras.io/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://jupyter.org/install.html).

### Data

The dataset used for this project was a subset of the publicly available [2018 International Skin Imaging Collaboration data](https://challenge.isic-archive.com/data/#2018), which consists of 2596 dermoscopic images and 2594 corresponding lesion border segmentation ground truth masks. Hair segmentation masks were obtained from [Wei et al.](https://doi.org/10.1016/j.patcog.2021.107994), which contains 288 masks. 

### Contact
Michelle Li - michelle.li851@duke.edu or michelleli1999@berkeley.edu

### Contributors
Michelle Li, Roger Chang, Yuncheng Duan, and Charlotte Roh
