# Bird Sound Representation Vector Learning Self-Supervised Encoder

This repository contains the code that Rafael Tinajero Ayala and Justin George designed to explore the BirdCLEF competition on Kaggle, 
which was the basis of their project for COMP576. The following depicts the files present in this repository and how they are relevant:

## Files Provided

### bird-audio-to-spectrogram-dataset.ipynb
This file contains the preprocessing steps for converting the bird audio data into spectrogram format. This allows for audio to be
presented in a visual format, and thus allows for image-based models to be used on the given data.

### bird-call-mae-test-heads.ipynb, bird-call-mae-test-heads-2.ipynb
These files contain the pipelines of creating the Masked Autoencoder model architectures with patches and training them on the
preprocessed spectrogram data. They differ in terms of how class balancing was addressed. 

### bird-call-vit-orig.ipynb, bird-call-vit-balance.ipynb
These files contain the pipelines of creating the Vision Transformer model architectures with patches and training them on the
preprocessed spectrogram data. They differ in terms of how class balancing was addressed, with "orig" not addressing it at all
and "balance" downsampling on classes with large sizes.

### result-plots.ipynb
This file creates visualizations of the results from the pipeline notebooks to be displayed within the report.
