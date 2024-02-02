
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>
1. Clone the repository:

  ```bash
  git clone https://github.com/dompio/dog_breed.git
  ```

2. Install conda as a stand-alone version [link](https://docs.conda.io/projects/miniconda/en/latest/)

3. Initialize conda `~/miniconda3/bin/conda init zsh`

4. Create venv `python3.8 -m venv domi_venv`

5. Activate venv `source domi_venv/bin/activate`

6. Specify python version for conda `conda install python=3.8`

7. Install tensorflow-deps with conda `conda install -c apple tensorflow-deps`

8. Install tensorflow following the instrucions for 2.12 `python -m pip install tensorflow-macos` https://developer.apple.com/metal/tensorflow-plugin/

9. Install tensorflow-metal plug-in `python -m pip install tensorflow-metal`

10. Install other reqirements via pip `pip install -r requirements/requirements.txt`
   
* The code should run using Python 3.*.
* Libraries used:
  ```
  opencv-python
  h5py
  numpy
  scipy
  tqdm
  keras
  scikit-learn
  pillow
  ipykernel
  matplotlib  
  ```

## Project Motivation<a name="motivation"></a>

In this project, the aim was to develop a dog breed classification system using Convolutional Neural Networks. Given an image of a dog, the algorithm identifies an estimate of the corresponding dog breed. If supplied an image of a human, the code supplies the resembling dog breed.

## Results <a name="results"></a>

In this project, I leveraged a dataset of labeled dog images provided by Udacity, consisting of various breeds. The steps to complete the project included preprocessing the data, splitting it into training, validation, and testing sets. I then designed and train a CNN model to learn the intricate features and patterns that distinguish one breed from another.

The CNN from scratch resulted in a test accuracy of 3.4255%, meeting the project criteria. The CNN using transfer learning greatly improved the accuracy, resulting in a test accuracy of 80.6220%. More can be found in the [Medium blog post](https://medium.com/@dominikapiosik/understanding-convolutional-neural-networks-cnns-for-dog-breed-classification-0fbb98c2934b).

## File Descriptions <a name="files"></a>

`dog_app.ipynb` Jupyter notebook with CNN implementation.

`extract_bottleneck_features.py` function to extract bottleneck features.

`bottleneck_features` folder contains bottleneck features for the chose architecture.

`data` folder contains human and dog images for training and validation.

`haarcascades` folder contains OpenCV pre-trained face detector in xml file.

`requirements` folder contains the requirements.txt file for running the code.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Images used for testing purposes above were obtained from [Unsplash](www.unsplash.com). 

Credits in the order in which they were used: 
*Photo by Houcine Ncib on Unsplash - https://unsplash.com/photos/smiling-woman-holding-cheek-B4TjXnI0Y2c
*Photo by Pavel Anoshin on Unsplash - https://unsplash.com/photos/derek-fisher-d0peGya6R5Y
*Photo by Milli on Unsplash - https://unsplash.com/photos/dogs-face-2l0CWTpcChI
*Photo by Victor Grabarczyk on Unsplash - https://unsplash.com/photos/black-and-white-short-coated-dog-N04FIfHhv_k
*Photo by Enis Yavuz on Unsplash - https://unsplash.com/photos/golden-retriever-on-gray-rock-during-daytime-KKtuRtGkDys
*Photo by Igor Son on Unsplash - https://unsplash.com/photos/green-leaf-plant-FV_PxCqgtwc
