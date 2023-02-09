# Authentication-System-using-LSTM-Action-Detection-and-MTCNN-Facial-Recognition
Machine-Learning-Based Authentication System using LSTM RNN Action Detection and MTCNN Custom Facial Recognition


# The Authentication System Consists of The Following Modules:

# 1) Action Detection Machine Learning Model based on the Long Short-Term Memory (LSTM) Recurrent Neural Network (RNN) Architecture 
The LSTM RNN action detection model is trained using Tensorflow and Keras machine learning frameworks where the dataset is based on right hand pose estimation keypoints  values which is collected manually using the Mediapipe holistic pipeline. The dataset consists of 6 classes which are hand signs of numbers from 0 to 5 and for each class 30 videos of 30 frames each have been collected. The overall system accuracy is 96.3% and it has 150,566 learnable parameters.

# 2) Human Pose Estimation of right hand using Mediapipe Holistics Pipeline
The Mediapipe holistics provide keypoints/ landmarks for the face, body (pose), and right and left hands. Only kepoints for the right hand has been extracted and used for the action detection model. The right hand has 21 keypoints and each keypoint consist of x, y, and z values which gives us a total of 63 values for each frame.

# 3) Facial Recognition using VGGFace2 Dataset for Face Recognition and MTCNN for Facial Features Extraction and Detection
The facial recognition module uses the VGGFace2 dataset and MTCNN algorithm to accurately detect and extract facial features for recognition purposes. The VGGFace2 pre-trained model has been trained on a large-scale face recognition dataset and can handle large variations in pose, age, illumination, ethnicity, and profession. The MTCNN algorithm is used to detect facial landmarks and improve the accuracy of the facial recognition process.

# 4) Text-To-Speech Module using pyttsx3 Python Library
The text-to-speech module uses the pyttsx3 Python library to convert text into spoken language. This module can be used to provide verbal feedback to users in the system interface.

# 5) System Interface GUI using Tkinter Python Library
The system interface GUI is created using the Tkinter Python library. This GUI provides an easy-to-use interface for users to interact with the authentication system. The GUI integrates all of the system modules, including the action detection and facial recognition modules, providing a seamless user experience. Additionally, the GUI is integrated with the text-to-speech module to provide verbal feedback to users, further enhancing their experience.

# 6) Serial Communication with Door Lock
The authentication system also includes serial communication with a door lock to control access. The system can communicate with the door lock through serial communication protocols. This integration allows the system to control the door lock and grant access based on successful authentication through the action detection and facial recognition modules.
