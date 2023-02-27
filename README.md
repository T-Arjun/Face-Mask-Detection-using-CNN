# Face-Mask-Detection-using-CNN

This code downloads the 'Face Mask Detection' dataset from Kaggle, extracts it and preprocesses it for training a machine learning model to detect if a person is wearing a mask or not.

# Import Libraries

    os: This library provides a way of using operating system dependent functionality.
    
    numpy: This library is used for working with arrays.
    
    matplotlib: This library is used for data visualization.
    
    cv2: This is a computer vision library.
    
    google.colab.patches: This library is used for displaying images in Google Colab.
    
    PIL: This library is used for opening, manipulating and saving images.
    
    sklearn: This library provides a collection of tools for machine learning model building and evaluation.
    
# Download and Extract Dataset

    kaggle: This library is used to download the dataset from Kaggle.
    ZipFile: This library is used to extract the downloaded zip file.
    Set up Kaggle API credentials to download the dataset from Kaggle.
    
    
 # Data Preprocessing

    Resize all images to (128, 128).
    Convert all images to RGB format.
    Loop through images in the 'with_mask' and 'without_mask' folders, and append them to a list 'data'.
    Add the corresponding labels to another list 'labels'. 'with_mask' images are labeled as 1, and 'without_mask' images are labeled as 0.
    Convert 'data' and 'labels' to numpy arrays 'X' and 'Y' respectively.
    Split 'X' and 'Y' into training and testing sets using the 'train_test_split' method from sklearn.
    Scale the pixel values of 'X_train' and 'X_test' by dividing them by 255.
