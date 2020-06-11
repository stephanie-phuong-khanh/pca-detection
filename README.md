# Prostate cancer detection with mp-MRI

Implementation of [Deep transfer learning-based prostate cancer classification using 3 Tesla multi-parametric MRI](https://pubmed.ncbi.nlm.nih.gov/30460529/)

Acquire and place data into `/data` folder.

Run `00_preprocess_t2.py` and `00_preprocess_adc.py` to crop and normalize images.

Run `01_organize.py` to augment data to organize lesion images with their labels, patient numbers, zones, etc.

Uses ResNet50 CNN pretrained on ImageNet.
