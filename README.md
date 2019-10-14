# Wildlife image classification

This notebook implements a CNN, using transfer learning (Xception architecture) to classify 14 classes of animals in the wild, based on Kaggle competition dataset: https://www.kaggle.com/c/iwildcam-2019-fgvc6/data

The notebook uses DLHelper API (https://github.com/LukasNorbutas/DLHelper) to tidy up and resize raw input images, build a train-validation-test split and train neural net models. Several features available in the API:
- Resize images in the train directory to decrease train time
- Build a train/test split using augmentation/downsampling/upsampling
- Resize/reaugment train images on the go (during training/between epochs/etc)
- Learning rate tools: find optimal learning rate using find_lr, discriminative learning rates (Adam), one-cycle-learning
