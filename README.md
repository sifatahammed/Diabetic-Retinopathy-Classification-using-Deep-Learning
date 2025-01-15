# Diabetic-Retinopathy-Severity-Classification-using-Deep-Learning
This project performs a comparative analysis of various deep learning models for classifying the severity of Diabetic Retinopathy (DR) using fundus images. The models evaluated include CNN, InceptionV3, ResNet50, DenseNet121, and EfficientNetB6. The performance of these models is assessed using accuracy and Cohen's Kappa score.

## Dataset



*   This project utilizes the [Kaggle Diabetic Retinopathy Detection]([dataset_link](https://www.kaggle.com/competitions/diabetic-retinopathy-detection/data)) dataset.
*   The dataset was composed of a large set of high-resolution retina images taken under a variety of imaging conditions. A left and right field is provided for every subject. Images are labeled with a subject id as well as either left or right (e.g. 1_left.jpeg is the left eye of patient id 1).

A clinician has rated the presence of diabetic retinopathy in each image on a scale of 0 to 4, according to the following scale:

*  0 - No DR
*  1 - Mild
*  2 - Moderate
*  3 - Severe
*  4 - Proliferative DR

## Models

The following pre-trained deep learning models were fine-tuned and evaluated:

*   **CNN (Custom CNN):** A custom convolutional neural network architecture. *Provide details if it's a specific architecture you designed.*
*   **InceptionV3:** A deep convolutional architecture known for its efficient use of computational resources.
*   **ResNet50:** A residual network architecture that addresses the vanishing gradient problem in deep networks.
*   **DenseNet121:** A densely connected convolutional network that promotes feature reuse.
*   **EfficientNetB6:** A family of models designed for optimal efficiency and accuracy.

## Evaluation Metrics

Model performance was evaluated using:

*   **Accuracy:** The overall percentage of correctly classified images.
*   **Cohen's Kappa Score:** A metric that measures inter-rater agreement, taking into account the possibility of agreement occurring by chance. This is particularly relevant for multi-class classification problems like DR severity grading.

## Project Structure
## Requirements

*The project requires the following Python libraries:

*  numpy
*  pandas
*  scikit-learn
*  tensorflow 
*  keras 
*  opencv-python
*  matplotlib
*  seaborn
*Install the requirements:

*  ```bash
*    pip install -r requirements.txt
* Create a requirements.txt file using pip freeze > requirements.txt after setting up your environment.

## Results
The experiments demonstrated the effectiveness of deep learning models for classifying DR severity.

* Key Findings:

*    Model Performance: The EfficientNetB6 model achieved the highest accuracy (89%), followed by ResNet50 (84%), CNN (82%), InceptionV3 (81%), and DenseNet121 (73%).
*    Cohen's Kappa: Include the Cohen's Kappa scores for each model here. For example: "EfficientNetB6 also achieved the highest Cohen's Kappa score of 0.85, indicating strong agreement between the model's predictions and the ground truth labels."
*   The confusion matrices (available in results/) show that DenseNet121 struggled to distinguish between 'Mild' and 'Moderate' DR, contributing to its lower overall performance."

Future Work
*  Explore data augmentation techniques to improve model robustness and generalization.
*  Investigate different loss functions and optimization strategies.
*  Evaluate the models on larger and more diverse datasets.
*  Deploy the best-performing model for real-world applications.
## Contributing
*Contributions are welcome! Please open an issue or submit a pull request.

## License
[MIT License]
