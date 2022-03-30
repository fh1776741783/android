# Requirements
PyTorch 1.10.1, torchvision 0.11.2. The code is tested with python=3.8, cuda=10.2.

# Train
## 1. Prepare training data 
Download the training sets and unzip them to `./trainsets/Flickr/Train`.
Download the val sets and unzip them to `./testsets/Flickr`.

Generate binaries

We pre-process the images before training. This step will decode all png files and save them as binaries.

```
python prepare/create_bin.py
```

Generate metric list by informative importance

```
python prepare/create_bin_ii.py
```

## 2. Begin to train
Run `train.py` to perform training.

# Test
## 1. Prepare test data 
Download the test sets and unzip them to `./testsets`. 

## 2. Begin to test
Run `test.py` to perform a demo inference. Results (.png files) will be saved to `./results`.
