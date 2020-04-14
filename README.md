# Offline Signature Verification on Real-World Documents
This is the official repository of our CVPRW2020 Biometrics Workshop paper "Offline Signature Verification on Real-World Documents". This repository contains Tobacco-800 Signature pairs to simulate a signature verification  

## Tobacco-800 Signature Pairs
All signatures that have been extracted from Tobacco-800 dataset [1] are named with page name used in annotations. Some signatures have been removed due to mislabeling and no valid ID issues. 

In author-ID-mappings.txt file we gave integer ID numbers for each labeled user in Tobacco-800 dataset. In annotations there are some signatures with missing userID. We did not use any signature of them. 

In tobacco_test_pairs.txt file, all positive and negative signature pairs have been written as
```
signature_path_1 signature_path_2 0/1
```
0 indicates negative pair (no match) and 1 indicates positive pair (match).
Also, all training, validation and test signatures with their names are in train.txt, val.txt and test.txt respectively.

Citation information of our paper will appear here after publication has been released. 

[1]: David Lewis, Gady Agam, Shlomo Argamon, Ophir Frieder,D Grossman, and Jefferson Heard. Building a test collectionfor complex document information processing.  InProceed-ings of the 29th annual International ACM SIGIR Confer-ence on Research and Development in Information Retrieval,pages 665–666, 2006
