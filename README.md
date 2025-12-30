# **🐠 Multiclass Fish Image Classification**

**1. Introduction**

The 'Multiclass Fish Image Classification' project aims to automatically identify the species of fish from given images using Deep Learning and Transfer Learning techniques. Image classification plays a vital role in aquaculture, marine research, and food industry automation. The main objective of this project is to build and evaluate various Convolutional Neural Network (CNN) architectures to determine which model delivers the best performance in classifying fish species accurately and efficiently.
The models explored include both custom CNNs and pre-trained models such as VGG16, ResNet50, MobileNetV2, InceptionV3, and EfficientNetB0. Each model was fine-tuned and tested to compare accuracy, loss, and generalization capability. The results obtained helped identify the optimal model for deployment through a Streamlit web application that can perform real-time predictions.

**2. Methodology**

The project followed a structured pipeline involving several stages to ensure a reliable and high-performing model:

**1.Data Preprocessing and Augmentation:** The dataset was normalized to the  [0, 1] range, and various data augmentation techniques such as image rotation, zooming, and horizontal flipping were applied to improve model robustness and prevent overfitting.

**2. Model Selection and Training:** The training phase involved experimenting with five pre-trained architectures (VGG16, ResNet50, MobileNetV2, InceptionV3, EfficientNetB0). Fine-tuning was performed on the fish dataset to adapt each model to the specific image features.

**3.Model Evaluation**: The models were evaluated based on accuracy and loss metrics using the final test set. Performance comparisons were made to determine the best-performing architecture.

**4.Deployment:** The final selected model was deployed as a Streamlit web application for real-time inference. Users can upload fish images, and the application predicts the species with confidence scores.


**3. Model Performance on Test Set**
   
Model Name	Test Accuracy	Test Loss
MobileNetV2	0.9820	0.0674
ResNet50	0.2595	2.0710
InceptionV3	0.9732	0.0957
EfficientNetB0	0.1641	2.3045
VGG16	0.7772	0.9956

**4. Analysis and Discussion**
   
Based on the evaluation, MobileNetV2 achieved the highest test accuracy (98.20%) and the lowest test loss (0.0674), indicating excellent learning and generalization capabilities. InceptionV3 followed closely with 97.32% accuracy, demonstrating strong performance but with a slightly higher loss. In contrast, models such as ResNet50 and EfficientNetB0 showed significantly lower accuracy, possibly due to hyperparameter mismatches or overfitting.
VGG16 achieved a moderate accuracy of 77.72%, suggesting it was able to learn meaningful features but struggled with deeper feature extraction compared to more modern architectures like MobileNetV2. Overall, MobileNetV2 proved to be both lightweight and highly accurate, making it an ideal candidate for real-time applications.

**5. Visualization Summary**
   
The training and validation accuracy plots showed consistent improvement with minimal overfitting for MobileNetV2 and InceptionV3. The confusion matrix analysis revealed that these models correctly classified most fish species, while minor misclassifications occurred in species with highly similar visual patterns.

**6. Conclusion**
    
The project successfully demonstrated how transfer learning can be effectively used for image classification tasks. **MobileNetV2** emerged as the best model with **98.20%** accuracy and a very low loss of **0.0674**, proving its efficiency for real-time deployment.

The developed Streamlit application allows end users to classify fish images instantly, enhancing automation possibilities in the fisheries and marine industries.

📈 Business / Research Impact
Domain	Practical Application
🌊 Marine Research	Automated fish species identification for biodiversity studies
🧾 Seafood Industry	Sorting and quality control in seafood processing lines
📱 Edge AI Systems	Deploy lightweight models like MobileNet for mobile or embedded cameras
💡 Scalable AI Framework	Reusable template for future datasets (e.g., fruits, plants, or medical images)
