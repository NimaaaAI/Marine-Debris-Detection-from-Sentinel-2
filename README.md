Abstract
This project focuses on using Artificial Intelligence to detect marine debris from various objects on the surface of oceans. The dataset used, known as MARIDA, is collected by the Sentinel-2 (S2) satellite over several years. The goal is to differentiate debris from other classes such as waves, ships, and foam. The MARIDA dataset is openly available for use with Machine Learning and Deep Learning algorithms, allowing for evaluation and comparison of their performance.

Introduction
Marine debris poses a significant threat to both human lives and the environment. Items like plastics can persist in oceans for extended periods, leading to various ecological and climate-related issues. To address this problem, the MARIDA dataset, collected by the S2 satellite, helps in identifying ocean debris. By leveraging Artificial Intelligence algorithms, such as Machine Learning and Deep Learning, we aim to accurately distinguish debris from other objects, thereby mitigating the impact of pollution on marine life and ecosystems.

Requirements and Data Analysis
A. Project Requirements
Annotated and split dataset from S2 satellite.
Availability of Machine Learning and Deep Learning algorithms.
Evaluation of algorithm performance.
Use of GPU for faster processing.
B. Dataset Overview
The MARIDA dataset spans seven years (2015-2021) and includes annotations for various objects observed by the S2 satellite. The dataset is already organized and annotated, making it suitable for direct use in training algorithms. It consists of 1381 patches with annotations for 15 classes, including Marine Debris, Dense Sargassum, Ships, and Clouds, among others.

C. Visualization
Visualization of patches using the rasterio library helps understand the dataset's structure and distribution of classes. Techniques like T-SNE (t-Distributed Stochastic Neighbor Embedding) aid in visualizing the distribution of classes in lower dimensions.

D. Data Preprocessing
Preprocessing involves tasks such as mapping dataset for labeling, splitting data into training, validation, and test sets, and handling the level of confidence associated with annotations. Shapefiles and histograms provide additional insights into the dataset's characteristics.

Algorithm Design using Spiral Approach
A. Decision Trees
Decision Trees offer transparency and interpretability, making them suitable for understanding classification processes. However, they may tend to overfit, requiring careful hyperparameter tuning. Regularizing techniques such as limiting the maximum depth of trees help prevent overfitting.

B. Random Forest
Random Forests address overfitting by employing multiple decision trees trained on different feature subsets. They excel in handling high-dimensional datasets like MARIDA and are less sensitive to the curse of dimensionality.

Consolidation of Performance and Future Plan
Evaluation of Decision Trees and Random Forests on the MARIDA dataset indicates Random Forests outperform Decision Trees. However, future plans involve exploring other architectures like YOLO for object detection within images to further improve detection accuracy.

Conclusion
The MARIDA dataset presents opportunities for effective marine debris detection using Artificial Intelligence. Both Decision Trees and Random Forests show promise in addressing this task, with Random Forests exhibiting better performance. Future work involves exploring advanced architectures to enhance detection capabilities further.

EU AI Regulation
Data Privacy and Ethics
Stricter rules may be imposed on data collection, processing, and sharing to ensure privacy rights are respected. Compliance with ethical guidelines for AI development and deployment may also be required.

Algorithm Transparency and Accountability
Regulations may demand transparency in algorithms used for marine debris detection, along with accountability for any errors or biases.

Safety and Environmental Impact
Assessment of AI systems' safety and environmental impact may be mandated to mitigate risks associated with misidentification of debris and other unintended consequences.

Certification and Compliance
Developers may need to obtain certification or demonstrate compliance with regulatory requirements before deploying AI models, involving rigorous testing and documentation of performance and safety measures.
