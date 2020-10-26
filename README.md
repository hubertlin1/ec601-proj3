# Project 3: Open Source

## SincNet
Since my topic for the term project is Multi-Speaker Identification, for this project I attempted to run and reproduce the results of SincNet, an open source neural architecture for audio processing.

### Dataset
The dataset used is the TIMIT corpus dataset, which provides a large set of raw recorded speech data sampled at 16000 Hz. The complete dataset can be found in the `TIMIT` directory.

### Data Preparation
A python script performs some preprocessing on the raw TIMIT data. In this process, amplitude normalization is performed and silences are removed from the beginning and end of speech recordings. The modified output follows the same directory structure as the original dataset and is stored in the `timit_output` directory.

### Reproduction of Results
Another python script runs an experiment to build and train the model using the data prepared in the previous step. In my case, I let the experiment run for a duration of 1500 epochs. This process took around 72 hours. The results are found in `exp/SincNet_TIMIT`. This includes the performance results over time and the final model.
