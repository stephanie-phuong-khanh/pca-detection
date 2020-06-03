# Prostate cancer detection with mp-MRI

Implementation of [Deep transfer learning-based prostate cancer classification using 3 Tesla multi-parametric MRI](https://pubmed.ncbi.nlm.nih.gov/30460529/)

Acquire and place data into `/data` folder.

Run `00_data_preprocess_t2.py` and `00_data_preprocess_adc.py` to crop and normalize images.

Run `01_data_augmentation.py` to augment data to increase model robustness and prevent overfitting.
