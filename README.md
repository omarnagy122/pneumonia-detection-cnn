# Pneumonia Detection from Chest X-Rays

Binary image classification (**Normal vs Pneumonia**) on chest X-ray images, comparing a **custom CNN** trained from scratch against **ResNet50 transfer learning** (ImageNet weights).

## What it does
- Loads the chest X-ray dataset from Google Drive and builds train / validation / test generators (128×128 images).
- Trains a custom CNN and a ResNet50-based model with `EarlyStopping` and `ModelCheckpoint`.
- Evaluates both on the test set (loss, accuracy, precision, recall), with confusion matrices and classification reports.
- Compares the two models side by side.

## Dataset
Not included (size). Download the *Chest X-Ray Images (Pneumonia)* dataset from Kaggle and place it as `chest_xray/{train,val,test}`, then update `base_dir` in the notebook.

## Stack
`TensorFlow / Keras` · `ResNet50` · `scikit-learn` · `Seaborn`

> Educational project only. Not a medical diagnostic tool.
