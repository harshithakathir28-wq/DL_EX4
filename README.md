# Experiment 4: Transfer Learning Using Pre-Trained Vision Models

## Aim

To implement transfer learning using a pre-trained vision model for image recognition and evaluate its performance on an image dataset.

## Tools and Technologies

* Python
* TensorFlow / Keras
* ResNet-50
* NumPy
* Matplotlib
* Google Colab
* CIFAR-10 Dataset
* Hugging Face
* GitHub

## Dataset

The CIFAR-10 dataset was used for image classification. It contains 60,000 color images of size 32 × 32 pixels belonging to 10 different classes.

### Classes

* Airplane
* Automobile
* Bird
* Cat
* Deer
* Dog
* Frog
* Horse
* Ship
* Truck

## Tasks Performed

### Task A – Dataset Preparation

* Loaded the CIFAR-10 dataset.
* Normalized image pixel values between 0 and 1.
* Split the training data into training and validation sets.
* Used the test dataset for final evaluation.
* Visualized sample images.

### Task B – Transfer Learning

* Loaded the pre-trained ResNet-50 model with ImageNet weights.
* Removed the original classification layer.
* Used Global Average Pooling.
* Added a Dense layer with 128 neurons.
* Added a Softmax output layer with 10 classes.
* Froze the pre-trained ResNet-50 layers.
* Compiled the model using the Adam optimizer and sparse categorical cross-entropy loss.

### Task C – Model Training and Evaluation

* Trained the transfer learning model for 10 epochs.
* Used a batch size of 64.
* Recorded training and validation accuracy.
* Recorded training and validation loss.
* Evaluated the model using the CIFAR-10 test dataset.
* Plotted accuracy and loss curves.

### Task D – Hugging Face Pre-Trained Models

* Explored pre-trained vision models available through Hugging Face.
* Performed image classification using a pre-trained vision model.
* Compared predictions with the transfer learning model.
* Documented observations.

## Model Architecture

ResNet-50 (Pre-trained) → Global Average Pooling → Dense Layer (128) → Softmax Output (10 Classes)

## Results

The transfer learning model successfully performed image classification on the CIFAR-10 dataset. Training and validation accuracy, loss curves, and testing accuracy were used to evaluate the model.

## Conclusion

Transfer learning using a pre-trained ResNet-50 model provides a faster and more efficient approach to image classification. The pre-trained model already contains useful visual features learned from a large dataset, reducing the amount of training required for the new task.
