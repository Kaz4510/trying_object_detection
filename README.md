# Computer Vision - object detection
A basic Object detection on images using Tensorflow, TFOD2 and OPENCV. The goal here is to explore labeling datasets and ML Liberaries.

# Step 1: Annotate the dataset
  
  Look for images (data) to train & test your model. For training, we need labeled images, i.e., labeled dataset. To create this, we will use labelImg, a python liberary created specifically for this purpose. Use the following command to download the liberary:
  
    pip install labelImg

  Through this, we need to upload the images, select the object and give a label. It looks something like this:
  
  ![labelimg_sample](https://github.com/user-attachments/assets/bde2ceec-2aa7-4638-b4f7-d3c4c50ff735)


# Step 2: Training model.
Follow the code files to understand more.
The model detects the presence on cars on an image using a custome trained model. For the pre trained model, only a single item is classified for training.
The final output is as follows:
![image](https://user-images.githubusercontent.com/60610819/230354386-e587d4c0-e3d6-4efe-84db-f1da79583280.png)
![image](https://user-images.githubusercontent.com/60610819/230354344-07803abc-4113-43b0-8a6c-1ea2dcdf6bc0.png)
![image](https://user-images.githubusercontent.com/60610819/230354575-1d5372aa-fc5e-4471-92b4-fded9ec7e05e.png)
![image](https://user-images.githubusercontent.com/60610819/230355100-01957dbc-83ff-47f0-b9a1-29acab19666f.png)

# Step 3: Augment the code to work with video input. 
initial idea:

    1. Input the video file
    2. Convert the video into seperate frames.
    3. Input the frames into the model, generate a report based on this input

Possible advancements:
  We could try to define an action like <<Walking, Swimming, Jumping>> by assiging a sequence frames to this label and run the model to detect this sequence.
  An easier and more convenient way of doing this is simply using OPENCV liberary. Read the file on video detection for this.
