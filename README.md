Image Classification: Detecting Presence of Sea

I built this project to classify images based on whether they contain the sea or not. The goal was to train a traditional machine learning model that could distinguish between images with sea and those without using custom handcrafted features.

The function raw_image_to_representation extracts several types of image representations, such as color histograms (HC), grayscale pixels (GC), raw pixel tensors (PX), Histogram of Oriented Gradients (HOG), and hybrid combinations like HOG + HC. These representations are used to build structured datasets through load_transform_label_train_dataset and load_transform_test_data, where each image is labeled as either "sea" or "non-sea" based on its folder or name.

The model training happens in learn_model_from_dataset, where I integrated support for Decision Trees, Random Forests, SVMs, Naive Bayes, k-NN, AdaBoost, XGBoost, and ensemble techniques like Voting and Stacking. Grid search and cross-validation are used for hyperparameter tuning.

This project is a practical exploration of classical ML techniques applied to image classification, focusing on the specific and interpretable task of sea detection without relying on deep learning. It’s flexible, modular, and designed for experimentation.
