>Overview :
 
This project, Sign Language to Speech Conversion using Machine Learning, enables the recognition of American Sign Language (ASL) gestures and converts them into spoken words or sentences. It is designed to bridge the communication gap for individuals who use sign language.

**Features** :
 
- Real-Time Recognition: Converts live webcam feed into recognized gestures.
- Robust Prediction: Implements stabilization for accurate gesture recognition.
- Word and Sentence Formation: Automatically forms words and sentences with proper segmentation (space and full stop gestures).
- Text-to-Speech Conversion: Speaks out the recognized text for better accessibility.
- User-Friendly GUI: Displays the current alphabet, word, and sentence in real time.

 **Tech Stack** :
 
* Languages: Python
* Libraries: MediaPipe, OpenCV, Tkinter, Pyttsx3, Scikit-learn
* Machine Learning Model: Random Forest Classifier

>How the Project Was Built
 
**Dataset Collection** :

* A custom dataset was created using the collectImgs.py script.
* For each gesture, 100 images were captured, ensuring diverse angles and lighting conditions for robust training.
* The dataset includes 38 classes, representing:
* 26 alphabets (A-Z)
* 10 digits (0-9)
* A gesture for space
* A gesture for full stop

**Feature Extraction and Preprocessing** :

- The collected images were processed using MediaPipe, extracting 21 key landmarks for each hand.
- Each landmark was converted into a normalized 2D coordinate (x, y), resulting in 42 features per sample.
- The preprocessed data was saved as a pickle file using the createDataset.py script.

**Model Training** :

- A Random Forest Classifier was used for training, offering high accuracy with fast training times.
- The dataset was split into training and testing sets (80-20 ratio).
- Training results showed high accuracy, ensuring reliable gesture recognition.
	
 **Inference and Real-Time Conversion** :

- The trained model was integrated into a real-time system using main.py.
- The system uses a stabilization buffer to improve gesture detection and avoids misclassifications.
- A Text-to-Speech (TTS) engine was used to convert recognized gestures into audible speech.
- A user-friendly GUI was built with Tkinter for better interaction.


**Future Enhancements** :
 
- Expand recognition to include dynamic gestures.
- Support for additional sign languages.
- Deploy the system as a mobile or web application for greater accessibility.
- Improve model accuracy with advanced deep learning techniques.

Thank You for reading this file. 

I hope you all understand this project.

>Best Regards :
**Animesh Kumar Srivastava**

[Follow for more project on Linkedin](https://www.linkedin.com/in/animeshkumar143/)

	- NoCopyright Animesh
