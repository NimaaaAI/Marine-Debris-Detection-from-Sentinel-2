<div align="center">
  <a href="https://marine-debris.github.io/">
    <img src="https://github.com/user-attachments/assets/f15600ec-bd0e-48ff-abd2-37ff2867d82e" alt="Marida" width="300">
  </a>
</div>

# Abstract
This project focuses on using Artificial Intelligence to detect marine debris from various objects on the surface of oceans. The dataset used, known as [MARIDA](https://github.com/marine-debris/marine-debris.github.io), is collected by the Sentinel-2 (S2) satellite over several years. The goal is to differentiate debris from other classes such as waves, ships, and foam. The MARIDA dataset is openly available for use with Machine Learning and Deep Learning algorithms, allowing for evaluation and comparison of their performance.

# Introduction
Marine debris poses a significant threat to both human lives and the environment. Items like plastics can persist in oceans for extended periods, leading to various ecological and climate-related issues. To address this problem, the MARIDA dataset, collected by the S2 satellite, helps in identifying ocean debris. By leveraging Artificial Intelligence algorithms, such as Machine Learning and Deep Learning, we aim to accurately distinguish debris from other objects, thereby mitigating the impact of pollution on marine life and ecosystems.

# Dataset Overview
The MARIDA dataset spans seven years (2015-2021) and includes annotations for various objects observed by the S2 satellite. The dataset is already organized and annotated, making it suitable for direct use in training algorithms. It consists of 1381 patches with annotations for 15 classes, including Marine Debris, Dense Sargassum, Ships, and Clouds, among others.

# **Project Overview**
- **Dataset Preparation** : Utilize annotated datasets from S2 satellite, ensuring a clear split for training, validation, and testing.
- **Algorithm Implementation and Comparison**: Explore and evaluate Machine Learning and Deep Learning algorithms to achieve optimal performance. 
- **Performance Evaluation**: Evaluates the accuracy, precision, and other relevant metrics of the applied models.  
- **Accelerated Processing**: Leverage GPUs to expedite computational tasks and model training.
- **Data Visualization**: Uses the `rasterio` library to visualize dataset patches, aiding in understanding the dataset structure and class distribution. Additionally, it applies dimensionality reduction techniques such as **T-SNE (t-Distributed Stochastic Neighbor Embedding)** to assist in visualizing class distributions in the lower-dimensional spaces.
- **Data Preprocessing**: Maps the dataset to corresponding labels for supervised learning and divides it into training, validation, and test sets. It also accounts for confidence levels in annotations to ensure high data quality. Additionally, shapefiles and histograms are utilized to gain deeper insights into the dataset's characteristics.
- **Algorithm Design Using Spiral Approach**: Algorithm development follows a spiral approach, beginning with simpler models like Decision Trees to establish a baseline and gradually increasing the complexity with models like Random Forest for refinement.  

  **Decision Trees** offer transparency and interpretability, making them ideal for the initial exploration of classification tasks. However, they are prone to overfitting, which requires careful hyperparameter tuning and the application of regularization techniques, such as limiting the tree depth.  

  **Random Forest**, built on an ensemble of decision trees, mitigates overfitting by aggregating the predictions from multiple trees. It handles high-dimensional datasets, such as the MARIDA dataset, efficiently and performs well across varied feature spaces, while being less sensitive to the curse of dimensionality, which ensures robustness with large datasets. However, Random Forest can be computationally expensive, especially with large datasets or when using numerous trees, and it may require careful tuning of hyperparameters, such as the number of trees and features considered at each split, to achieve optimal performance.
- **Performance Consolidation & Future Plans**: Indicates that Random Forest offers better performance than Decision Trees on the MARIDA dataset, providing improved generalization and higher accuracy. Additionally, it suggests exploring advanced architectures, such as YOLO, for object detection to enhance detection accuracy in images.

# Conclusion
The MARIDA dataset presents opportunities for effective marine debris detection using Artificial Intelligence. Both Decision Trees and Random Forests show promise in addressing this task, with Random Forests exhibiting better performance. Future work involves exploring advanced architectures to enhance detection capabilities further.

# **EU AI Regulation Overview**  
The European Union is likely to enforce comprehensive regulations to ensure responsible AI development and deployment. These regulations are designed to address various aspects of AI systems, including data privacy, algorithm transparency, safety, and compliance. Below are the key areas covered under the EU AI Regulation:

- **Data Privacy and Ethics**: Stricter rules will be imposed on data collection, processing, and sharing to protect privacy rights. Additionally, AI development must comply with ethical guidelines to ensure the responsible use of technology.

- **Algorithm Transparency and Accountability**: AI systems, such as those used for marine debris detection, will be required to maintain transparency in their algorithms. Developers will be held accountable for any errors, biases, or unintended consequences produced by the algorithms.

- **Safety and Environmental Impact**: AI systems will need to undergo assessments to ensure they are safe for deployment and do not have negative environmental impacts. This is particularly important to avoid risks like misidentification of marine debris or other unintended consequences.

- **Certification and Compliance**: Developers will need to demonstrate compliance with regulatory requirements, possibly including obtaining certifications before deploying AI models. This would involve rigorous testing, documentation, and validation of the models' performance and safety measures.
