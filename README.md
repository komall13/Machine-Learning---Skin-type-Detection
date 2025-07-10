# Machine-Learning---Skin-type-Detection
Skin Type Detection using Machine Learning
This project focuses on building a machine learning model that detects human skin type (Oily, Dry, Normal) based on image data. The model is trained and evaluated using a structured dataset of facial skin photographs, and the implementation is done entirely in Google Colab using Python and TensorFlow/Keras.

###Dataset Structure
The dataset is organized into three main folders:
/dataset
│
├── train/          ← Contains training images (not uploaded to GitHub due to size)
│   ├── oily/
│   ├── dry/
│   └── normal/
│
├── valid/          ← Validation images (uploaded to GitHub)
│   ├── oily/
│   ├── dry/
│   └── normal/
│
└── test/           ← Test images (uploaded to GitHub)
    ├── oily/
    ├── dry/
    └── normal/
Each subfolder (oily, dry, normal) contains skin type photographs, and the folder name represents the corresponding label for classification.

###Project Workflow
Data Preprocessing:
Images are loaded using Keras ImageDataGenerator for real-time data augmentation.
Data is normalized and resized for model compatibility.

Model Building:
A Convolutional Neural Network (CNN) architecture is used.
The model is compiled using categorical_crossentropy as the loss function.

Training:
Training is performed on the /train folder (locally or via Colab file upload).
Validation is done on the /valid folder.

Testing:
Final accuracy and performance metrics are evaluated on the /test folder.

###GitHub Note
Due to file size limitations, only the test/ and valid/ folders are uploaded to this repository.
The train/ folder can be manually uploaded in Google Colab when running the notebook.

###Results
The model successfully classifies images into three skin types: Oily, Dry, and Normal.
Accuracy and loss metrics are displayed during training and evaluation.
