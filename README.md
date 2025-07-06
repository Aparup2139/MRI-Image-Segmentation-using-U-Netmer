<h1>UNetmer Brain MRI Tumor Segmentation<h1>

This project implements a brain MRI tumor segmentation model using UNetmer, a hybrid deep learning architecture combining U-Net and Transformer components. The model is trained on the LGG MRI Segmentation dataset from Kaggle, designed to segment tumors in MRI images while addressing class imbalance (small tumor regions). The project is optimized for Kaggle’s P100 GPU environment and includes data preprocessing, model training, evaluation metrics, and visualizations, meeting the requirements of a hackathon focused on medical image segmentation.

Features





UNetmer Model: Integrates U-Net’s local feature extraction with a Transformer’s global context for robust tumor segmentation.



Dataset Handling: Processes the LGG MRI dataset with a 70-21-9 train-val-test split, using Albumentations for preprocessing (resize, normalization) and augmentation (flips, brightness, rotation).



Evaluation Metrics: Computes IoU, Recall, F1 for the tumor class, overall accuracy, macro-averaged IoU, and confusion matrix, as required by the hackathon.



Visualizations:





Data verification: Displays sample MRI images, highlighted abnormalities, and masks (data_check.png).



Evaluation: Shows input image, ground truth, predicted mask, and confusion matrix with metrics (results.png).



Kaggle-Optimized: Runs efficiently on Kaggle’s P100 GPU with batch size 4 and 224x224 images.
