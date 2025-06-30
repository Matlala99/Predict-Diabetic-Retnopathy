//use this link to download the dataset
https://drive.google.com/drive/folders/1aEAowEDGh9luzgUnVGLu3Dubm8ZpWt4K?usp=sharing


Diabetic Retinopathy Detection Using Deep Learning
Project Overview
This project leverages deep learning to automate the detection and classification of diabetic retinopathy (DR) from retinal fundus images. DR is a severe complication of diabetes that can lead to vision loss if not detected early. The goal is to classify retinal images into five severity levels: No_DR, Mild, Moderate, Severe, and Proliferative_DR. The project employs transfer learning with pre-trained convolutional neural networks (CNNs) and uses Grad-CAM visualizations to enhance model interpretability.

Key Features
Model Architecture: Utilizes MobileNetV2, selected for its balance of accuracy and computational efficiency.

Performance: Achieves 95.10% accuracy in classifying DR severity levels.

Interpretability: Incorporates Grad-CAM to visualize regions of the retina influencing predictions, ensuring clinical relevance.

Preprocessing: Includes Gaussian filtering, resizing, normalization, and data augmentation to enhance model robustness.

Dataset
The dataset consists of retinal fundus images categorized into five classes:

No_DR: Healthy retina.

Mild: Early signs like microaneurysms.

Moderate: Hemorrhages and hard exudates.

Severe: Multiple hemorrhages and microvascular abnormalities.

Proliferative_DR: Advanced stage with neovascularization.

Methodology
Preprocessing: Noise reduction, resizing, normalization, and augmentation.

Model Training: Evaluated 27 pre-trained CNNs; MobileNetV2 was selected.

Training Pipeline:

Data splitting (80% training, 20% validation).

Augmentation (rotations, flips, scaling, brightness adjustments).

Optimization using the Adam optimizer and dynamic learning rate scheduling.

Evaluation Metrics: Accuracy, precision, recall, and F1-score.

Interpretability: Grad-CAM heatmaps to validate model focus on clinically relevant features.

Results
High accuracy (95.10%) with strong performance for No_DR and Proliferative_DR classes.

Challenges in distinguishing Mild and Moderate cases due to visual similarities.

Grad-CAM confirmed the model's focus on pathological features like hemorrhages and neovascularization.

Challenges
Class Imbalance: Disproportionate representation of No_DR cases.

Intermediate Class Overlap: Difficulty in distinguishing Mild and Moderate stages.

Dataset Diversity: Limited representation of diverse demographics and imaging conditions.

Future Directions
Address class imbalance using synthetic oversampling (e.g., SMOTE or GANs).

Experiment with ensemble models (e.g., combining MobileNetV2 and EfficientNet).

Improve generalizability through domain adaptation and transfer learning.

Enhance interpretability with complementary techniques like LIME.

Broader Implications
This project demonstrates the potential of AI to:

Scale DR screening in resource-limited settings.

Reduce the burden on ophthalmologists by automating routine diagnostics.

Foster trust in AI through interpretable predictions.
