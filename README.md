Developed a multi-class image classification model to categorize shoe images into three brands (Nike, Adidas, Converse) using a dataset of 600 training images and 90 validation images.
Employed transfer learning with EfficientNet-B0 (pre-trained on ImageNet) as the backbone CNN architecture, customizing the classifier with dropout, ReLU activation, and fully connected layers for improved generalization.
Implemented data preprocessing and augmentation techniques (e.g., random resizing, flipping, rotation, color jittering, normalization) using torchvision transforms to enhance model robustness.
Conducted hyperparameter tuning via scikit-learn's ParameterGrid, evaluating combinations of learning rates (0.001–0.1), batch sizes (16–64), dropout rates (0.1–0.5), epochs (10), and weight decay (0–0.001), resulting in a tuning results table with train/validation accuracies.
Trained the model with PyTorch on Google Colab (GPU-accelerated), using AdamW optimizer, CrossEntropyLoss, and OneCycleLR scheduler; achieved a best validation accuracy of 93.33% on the held-out set.
Saved the optimized model (.pth format) and included a dedicated code cell for loading and testing on new data, ensuring reproducibility.

Technologies: Python, PyTorch, torchvision, scikit-learn, NumPy, Matplotlib, Google Colab

