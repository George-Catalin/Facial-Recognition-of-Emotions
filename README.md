# Facial-Recognition-of-Emotions
In order to run this program tensorflow 2.0 is needed, opencv, tqdm and numpy
# Steps to make the program work
       1. changing the path of facecascade in the config file
       2. python face_capture.py --emotion_name smile --number_of_images 200 to create the database. All the emotions must be done.
       This will open a camera that will take pictures of the users face expressing a certain emotion on the emotion stated when the program was ran ( in this case "smile" expressing happiness ).
       3. python dataset_creator.py
       We are using this because we are creating our own data. ( this could be done by just getting data from the internet, however this is free and simple ). It will transform the pictures in batches suitable for training the AI.
       4. python trainerr.py
       This is the part where we train the AI with the data we have made. Depending on how many pictures have been taken, it will take some time to train. To make the program accurate it is required to have pictures of different individuals and in different light conditions.
       5. python predictorr.py
       In the end, this will open up the camera and will start taking the video feed live. 
# DEMO
Notice that the program was trained just on data with my face and it can also detect the emotion of other people, with only 200 pictures of each expression. Managed to get really good results, but it is not 100% accurate.
Here is the link: https://www.youtube.com/watch?v=5xdkjhWTYqM
