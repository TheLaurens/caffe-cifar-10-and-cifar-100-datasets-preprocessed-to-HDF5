# Caffe cifar-10 and cifar-100 datasets preprocessed to HDF5 (can be opened in PyCaffe with h5py)
Both deep learning datasets can be imported in python directly with h5py (HDF5 format) or converted with a script to then be imported.

***NOTE: The training set has been shuffled and put in a big single batch, it was originally splitted into 5 files and not shuffled. The test set has not been shuffled and remained intact.***

## A. Direct import in caffe
You can simply download the zip file for the desired dataset and ignore the rest of this repository.

## B. Download and convert manually with the Python script
You can run my python script for the desired dataset. This way, you will not need to download the whole repository, but only the desired python script. It will automatically download and convert the dataset for caffe in the respective subfolder.
My script, however, has many python dependencies, if you can `import caffe` in python, you should normally have all the required libs, although caffe is never imported in the scripts I provide.

### Not shuffling datasets
If you do not want the datasets to be shuffled, my scripts can be a good starting point for the conversion of the cifar 10 and 100 datasets to the HDF5 caffe format. You may refer to this interesting tutorial to understand better how to do the conversion: https://github.com/BVLC/caffe/blob/master/examples/02-brewing-logreg.ipynb

## Link to original dataset
https://www.cs.toronto.edu/~kriz/cifar.html