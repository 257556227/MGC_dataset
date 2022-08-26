# Music genre classification
Source code and dataset of the our paper "Music Genre Classification Based on Fusing Audio and Lyric Information"

- Overview
- Dataset
- Baselines
- Algorithm

## Overview
![overview](https://user-images.githubusercontent.com/80112749/186842601-78c7851d-840b-4158-a5bc-3d039f872f4c.png)

## Dataset
We present the MGC Hybrid Fusion Dataset, a new open dataset for music genre classification. We built the dataset ourselves, which is the corresponding songs retrieved and downloaded from music websites using the songs from the mertroLyrics dataset on Kaggle and the song title information. The dataset contains 5,000 songs from folk, metal, country, hip-hop and jazz. We provide raw audio in mp3 format, the extracted audio features and the corresponding lyrics dataset.

### This data set will be published after our paper is received.

## Baselines
### 1. The single-modal methods
- [Zhang’s](https://doi.org/10.21437/interspeech.2016-1236) : A CNN network with maximum pooling, average pooling and residual structure was used for audio classification based on the STFT spectrogram of audio. <Improved music genre classification with convolutional neural networks>
- [Pons’s](https://doi.org/10.48550/arXiv.1711.02520) : Based on the STFT spectrogram of audio, convolution filters of different sizes were used in the time and frequency directions to extract information in the time-frequency domain, and the three-layer dense base with residual structure was used as the classifier. <End-to-end learning for music audio tagging at scale.>
- [Coban’s](https://doi.org/10.1109/siu.2016.7495686) : BOW was used to represent the lyric vector, and SVM was used to implement the classification. <Music genre classification from turkish lyrics>
- [Alexandros’s](https://doi.org/10.48550/arXiv.1707.04678) : A hierarchical attention structure was used to extract and classify the semantic information of the lyrics. <Lyrics-based music genre classification using a hierarchical attention network>
- [Kumar’s](https://doi.org/10.1109/icacci.2018.8554816) : BOW with TF-IDF weighting was used as the word embedding method, and multilayer perceptron was used as the classifier. <Genre classification using word embeddings and deep learning>
- [Neforawati’s](https://doi.org/10.1109/IC2IE47452.2019.8940826) : The word embedding methods BOW and word2vec are used, and the LSTM network was used as the classifier. <Indonesian lyrics classification using feature level fusion>

### 2. The multimodal methods
- [Kamtue’s](https://doi.org/10.1109/ICSEC47112.2019.8974740) : A CNN network similar to <End-to-end learning for music audio tagging at scale> was used to extract the sound quality features, BOW was used to embed the lyric word vector and an early fusion of the feature mosaic was implemented. <Lukthung classification using neural networks on lyrics and audios>
- [Wadhwa’s](https://doi.org/10.1109/GHCI50508.2021.9514020) : A fully symmetric architecture DCN was used to fuse the features of audio and lyrics. <Music genre classification using multi-modal deep learning based fusion>
- [Manco’s](https://doi.org/10.1109/ICASSP43922.2022.9746996) : ViLBERT was used for audio-linguistic pretraining to initialize part of the network. After pretraining, the audio backbone of the model was transferred to a set of music audio classification and regression tasks. < Learning music audio representations via weak language supervision>

## Algorithm
![Algorithm](https://user-images.githubusercontent.com/80112749/186843005-e92e602b-3056-4ab0-861a-f0fe5b37c149.png)
