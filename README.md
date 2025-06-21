# plaque-rupture-ai
Initial upload of AI model for plaque rupture

AI Model for Predicting Plaque Rupture (CNN + VGG16)

This is a Convolutional Neural Network (CNN)-based binary classification model built using TensorFlow and VGG16 to predict potential plaque rupture in coronary artery images.
Developed entirely in Google Colab, this project was independently created as part of a self-directed research initiative on AI in cardiology.

 Dataset
 
Custom dataset of coronary angiographic images (n = 12)

Located in: /plaque_dataset/ folder on Google Drive

Preprocessed and augmented using ImageDataGenerator

Model Architecture

Pre-trained VGG16 (frozen conv layers)

Custom top layers:

GlobalAveragePooling2D

Dense(128) + Dropout(0.5)

Dense(1, activation='sigmoid')

 Training
 
Loss function: binary_crossentropy

Optimizer: adam

Metrics: accuracy

Includes EarlyStopping to prevent overfitting

Output

Accuracy/Loss plots are generated post-training

Model shows improving training accuracy but limited generalization — due to small dataset size

Validation accuracy plateaued at ~50%, reflecting dataset limitations but promising architecture

 Key Challenges
 
Small dataset (n=12) limited learning and generalization

No institutional or lab support — built and coded entirely independently

Next steps include:

Increasing data volume

Trying fine-tuned transfer learning

Exploring ensemble models

 Related Work
 
 Published Research Paper on AI in Plaque Rupture Prediction: https://doi.org/10.58445/rars.2578 
(explores clinical context, limitations, and future directions)

 Author
 
Athira Gopan
CBSE '26

Note for Reviewers

This model was created in an academic setting with no institutional coding mentorship or research support. Its goal is not production accuracy, but proof of concept and initiative toward applying AI in early cardiac risk detection.
