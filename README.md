# Prostate cancer detection with mp-MRI

Implementation of [Deep transfer learning-based prostate cancer classification using 3 Tesla multi-parametric MRI](https://pubmed.ncbi.nlm.nih.gov/30460529/)

Acquire and place data into `/data` folder.

Run `00_preprocess_t2.py` and `00_preprocess_adc.py` to crop and normalize images. Run `01_organize_data.py` to augment data to organize lesion images with their labels, patient numbers, zones, etc.

Uses ResNet50 CNN pretrained on ImageNet. Run `02_dtl_adc.py` and `02_dtl_t2.py` to train and run model for ADC and T2 SPACE separately. Run `03_dtl_t2+adc.py` for model that takes as input ADC and T2 SPACE images, lesion zone, and T2 original lesion size.
