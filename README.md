# Skin Condition Classification Project
Phase 4 Project for Flatiron school's Data Science Live curriculum

This project uses a dataset of images of six different skin conditions, which can be found on [this Kaggle page](https://www.kaggle.com/datasets/syedalinaqvi/augmented-skin-conditions-image-dataset/data).

# Dataset Overview
---

The following description of the dataset was taken from the Kaggle page.

>**Description**:
>
>This dataset contains augmented images of six different dermatological conditions. Each category includes 399 images, providing a balanced >dataset ideal for training machine learning models, particularly in the field of medical image analysis.
>
>**Categories**:
>
>Acne: A common skin condition that occurs when hair follicles become clogged with oil and dead skin cells, leading to pimples, blackheads, or whiteheads.
>
>Carcinoma: A type of skin cancer that begins in the basal or squamous cells. The images in this category may show various stages and forms of skin carcinoma.
>
>Eczema: A condition that makes the skin red, inflamed, itchy, and sometimes results in blisters. The images depict different manifestations of eczema.
>
>Keratosis: A skin condition characterized by rough, scaly patches on the skin caused by excessive growth of keratin. This category includes images of various types of keratosis, such as actinic keratosis.
>
>Milia: Small, white, benign bumps that typically appear on the face, especially around the eyes and on the cheeks. The images show different instances of this condition.
>
>Rosacea: A chronic skin condition that causes redness and visible blood vessels in your face. This category contains images depicting the typical characteristics of rosacea.
>
>
>**Dataset Details**:
>
>Total Images: 2,394
>
>Images per Category: 399
>
>Image Format: JPEG
>
>Image Size: Variable.
>
>Augmentation Techniques: The images have been augmented using techniques such as rotation, flipping, zooming, and brightness adjustment to enhance the diversity of the dataset and improve model generalization.

In this project, I explore, analyze, and predict classifications of images of different skin conditons. The project is broken down into two different Jupyter Notebooks:
1. A technical *analysis* notebook - `skin_condition_technical_analysis.ipynb`
2. A technical *modeling* notebook - `skin_condition_technical_modeling.ipynb`

In the technical analysis notebook, I perform some exploratory data analysis on the dataset and visualize several attributes of the images, such as resolutions of images or the RGB channel intensities for images in each category.

![image](https://github.com/user-attachments/assets/a8572b3e-72a1-4577-8771-c5a1882a7e82)

Since this dataset is only comprised of images, the EDA is not quite as extensive as an EDA for a tabular dataset might be.

In the modeling notebook, I walk through the process of preprocessing the images for classification and creating a model to predict the different skin conditons. I explore two different approaches to modeling: a classical machine learning approach using the Histogram of Oriented Gradients (HOG), and a convolutional neural network approach using a custom architecture.

![image](https://github.com/user-attachments/assets/aeb59e44-2147-4e72-b23f-c11122483c2d)

The HOG approach yielded an accuracy score of approximately 60%.

![image](https://github.com/user-attachments/assets/564504c6-bbd3-4857-bcac-9b6b7124a347)

The convolutional neural network approach yielded an accuracy score of approximately 73%, which shows a 13% improvement from a classical machine learning approach.
