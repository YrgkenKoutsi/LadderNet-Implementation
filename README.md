* This implementation is based on [juntang-zhuang implementation](https://github.com/juntang-zhuang/LadderNet) and [orobix implementation](https://github.com/orobix/retina-unet). The main differences are the use of different datasets however, this is still under progress and not all the files have been updated as of this date.

# Requirement
* Python3.8
* PyTorch 0.4
* configparser
* h5py
* Pillow
* cv2

# How to run
* run ```python prepare_datasets_DRIVE.py``` to generate hdf5 file of training data
* run ```cd src```
* run ```python retinaNN_training.py``` to train
* run ```python retinaNN_predict.py``` to test

# Parameter defination
* parameters (path, patch size, et al.) are defined in <b>"configuration.txt"</b>
* training parameters are defined in src/retinaNN_training.py line 49 t 84 with notes <b>"=====Define parameters here =========" </b>

# Pretrained weights
* pretrained weights are stored in <b>"src/checkpoint"</b>
* results are stored in <b>"test/"</b>



### **Note that there might be issues on running the prediction model as i am currently undergoing changes in the dataset. However if you are familiar with LadderNet you should be just fine. If you want to test the model i would suggest checking [author](https://github.com/juntang-zhuang/LadderNet) or just wait a few days for the repository to be updated.**
