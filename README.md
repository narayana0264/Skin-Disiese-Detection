**Overview**
The objective of this project is to develop an AI model capable of detecting and classifying 10 different types of skin diseases:

Acne
Eczema
Psoriasis
Rosacea
Raynaud's phenomenon
Skin cancer
Scabies
Ringworm
Warts
Chickenpox
This project uses a custom implementation of the YOLOv9 object detection model. The neural network layers have been customized with ReLU activation functions to enhance learning. The final model is trained and evaluated using the Roboflow platform for dataset management and is deployed using TensorFlow/Keras for further use in various applications.


**Dataset**
The dataset used for this project is sourced from Roboflow, containing annotated images of various skin conditions. The dataset is divided into training, validation, and test sets. It is downloaded directly within the code using the Roboflow API.

**Model Architecture**
This project utilizes the YOLOv9 architecture for object detection with the following customizations:
ReLU Activation: ReLU layers have been inserted into the neural network to add non-linearity and aid in the learning process.

**Training**
The model is trained for 50 epochs with a batch size of 16. The training script is included in this repository, and the model is saved in Google Drive.

**Evaluation**
The model is evaluated using metrics such as precision, recall, mAP, and F1 score. The evaluation is performed on a separate validation dataset.

**Model Conversion**
After training, the PyTorch model is converted into TensorFlow’s .h5 format using ONNX. This step allows for easier deployment in environments that support TensorFlow.

**Results**
After training, the best model is saved, and evaluation metrics are logged. The model has shown promising results in identifying skin diseases with high accuracy.

**Usage**
Once trained, the model can be used for inference on new images. You can load the saved weights and use the model to predict skin conditions on unseen data.



