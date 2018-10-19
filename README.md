# FaceNet_FaceRecognition
Real Time Face Recognition by FaceNet

This application used the [FaceNet](https://github.com/davidsandberg/facenet) library of [@davidsandberg](https://github.com/davidsandberg) 
to implement the real time face recognition on the your computer's camera. This implementation made several changes to ```face.py``` and ```real_time_face_recognition.py```.
to adapt to this modification.

### The general procedures are:
1. Detect faces and their landmarks in video input stream by MTCNN.
2. Align detected face images.
3. Contruct embeddings for each of these face images.
4. Construct an embedding database of people you want to recognise.
5. Compare these face embeddings with your embedding database and find the matching person.

### To run this application:
0. Download the pre-trained model [20180402-114759](https://drive.google.com/file/d/1EXPBSXwTaqrSC0OhUdXNmKSh9qJUQ55-/view) to folder ```model_checkpoints/```
1. Make a folder of images of people you want to recognise (one person for each image) and
name the images with respect to the corresponding people. 
2. Clone the repository to your local computer.
3. Install the library and framework requirements and set up the ```PYTHONPATH``` variable to the ```src/``` folder.
4. In ```distributed/real_time_face_recognition.py```, provide the full path of the image folder you created earlider to variable ```img_folder```
5. Run the python file with command ```C:\...distributed> python real_time_face_recognition.py```

### Results:
![recognition_snap1](https://user-images.githubusercontent.com/18170028/47221388-da9f8580-d3bc-11e8-9751-3b6ce967817a.jpg)
![recognition_snap](https://user-images.githubusercontent.com/18170028/47221400-e25f2a00-d3bc-11e8-97cf-79dbd4cdd3f1.jpg)
![me_mom](https://user-images.githubusercontent.com/18170028/47221410-e5f2b100-d3bc-11e8-8f41-6f55c696ba34.png)

