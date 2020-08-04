# Offline Signature Verification on Real-World Documents
This is the official repository of our CVPR 2020 Biometrics Workshop paper "Offline Signature Verification on Real-World Documents". This repository contains Tobacco-800 dataset signature pairs to simulate a signature verification setup. Tobacco-800 is not focuses on signature verification but it contains real world documents with signatures. Therefore, we structured the signature pairs by using author informations to create a signature verification setup.  

## Tobacco-800 Signature Pairs
All signatures that have been extracted from Tobacco-800 dataset [1] are named with page name used in annotations. Some signatures have been removed due to mislabeling and no valid ID issues. 

In author-ID-mappings.txt file we gave integer ID numbers for each labeled user in Tobacco-800 dataset. In annotations there are some signatures with missing userID. We did not use any signature of them. 

In tobacco_test_pairs.txt file, all positive and negative signature pairs have been written as
```
signature_path_1 signature_path_2 0/1
```
0 indicates negative pair (no match) and 1 indicates positive pair (match).
Also, all training, validation and test signature ids used in training process of the network are in classification_train.txt, classification_val.txt, classification_test.txt respectively.

If you use this setup on your research, please cite our paper which presents this work.
```
@InProceedings{Engin_2020_CVPR_Workshops,
author = {Engin, Deniz and Kantarci, Alperen and Arslan, Secil and Ekenel, Hazim Kemal},
title = {Offline Signature Verification on Real-World Documents},
booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2020}
} 
```

[1]: David Lewis, Gady Agam, Shlomo Argamon, Ophir Frieder,D Grossman, and Jefferson Heard. Building a test collectionfor complex document information processing.  InProceed-ings of the 29th annual International ACM SIGIR Confer-ence on Research and Development in Information Retrieval,pages 665–666, 2006
