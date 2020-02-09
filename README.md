# Attendance Using Face Recognition

  > The Face-Recognition Software is done using the [face_recognition](https://pypi.org/project/face_recognition/) library which requires [dlib](http://dlib.net), the C++ based machine learning and deep learning module.

## Installation  
  - The Software is written in Python 3.6
  - All the required modules are in the requirement text file   
  `pip install requirement.txt`
  - or Execute the following **Command** to install the modules.   
  `pip install matplotlib numpy Pillow Click tox flake8 cmake dlib==19.8.1 sklearn face_recognition_models face_recognition opencv-contrib-python`
  - For creating a conda environment, the environment.yml file has all the requirement. The following command should be executed on anaconda prompt
  `conda env create -f environment.yml`
  where **environment.yml** is the path of the environment file.
  
## Working Procedure  
  - Upload the face data (Images) in **Folders** at the `Data/Train` Path. The Folder Names will be the labels of the Person in the images.  
  ![Data Structure](https://github.com/Immortalv5/Face-Recognition/blob/master/IMG/Data%20Structure.png)
  - Run `Train.py` for training the classifier which uses [KNN](https://scikit-learn.org/stable/modules/neighbors.html) (K- Nearest Neighbors Algorithm).
  - The Classifier is saved in `Model/` directory in `.clf` format.
  - By running `Video_Capture.py`, the video starts to stream from the choosen camera and labels the faces in the live stream.
  - If it finds an unknown face, it takes a snap and store it in the `\Noobie` directory.  
  ![Unknown](https://github.com/Immortalv5/Face-Recognition/blob/master/IMG/Unknown.png)
  
## Results
> If the Video display module is turned off, the software gives the list of people it recognized and how accurate it is in a command line.  

  ![Results](https://github.com/Immortalv5/Face-Recognition/blob/master/IMG/Results.png)
## Conclusion
> The Face_Recognition Software can be used for many applications. I have createed this for **Attendence System Based on Face Recognition**, for getting staff attendance. It can also be used as **Security** purpose.  
