# Towards-Deep-Learning-Based-Intrusion-Detection-in-IoT-Networks

**Objective:** The goal of this project is to develop an effective intrusion detection system (IDS) for IoT networks using deep learning techniques, specifically employing LSTM (Long Short-Term Memory) networks for category and subcategory prediction of network traffic.

**Problem Statement:** IoT networks face increasing security threats, necessitating robust intrusion detection mechanisms. Traditional methods often struggle with the dynamic and diverse nature of IoT traffic. Deep learning offers a promising approach to address these challenges by automatically learning and detecting patterns indicative of malicious activities.

**Dataset and Preprocessing:**

**Dataset:** Used the UNSW 2018 IoT Botnet dataset, which contains network traffic data labeled with categories and subcategories of attacks.

**Preprocessing:**
IP addresses were correctly parsed using the ipaddress library.
Categorical variables like 'proto' were encoded numerically using LabelEncoder.
Numeric features were scaled using StandardScaler.
Missing values were filled with zeros to ensure completeness.

**Modeling:**

**Autoencoder for Feature Extraction:**

Implemented a shallow autoencoder to learn compact representations of network traffic features.
Encoder part of the autoencoder was extracted to obtain encoded representations of the data.
LSTM Models for Prediction:

**Category Prediction:**
Utilized an LSTM network to predict the category of network traffic (e.g., normal traffic or different types of attacks).
Achieved using sparse_categorical_crossentropy loss for multi-class classification.
Subcategory Prediction:
Employed another LSTM network to predict subcategories of attacks within each category.
Used sparse_categorical_crossentropy loss for multi-class classification.

**Evaluation and Results:**

**Model Performance:**

Evaluated both LSTM models on test data, reporting accuracy metrics and generating classification reports.
Plotted training and validation accuracy/loss curves to visualize model performance and training dynamics.

**Outcome:**

Successfully trained LSTM models that demonstrated high accuracy in predicting intrusion categories and subcategories based on encoded network traffic features.
The models provide a basis for effective intrusion detection in IoT networks, enabling proactive security measures against potential threats.

**Key Contributions:**

**Deep Learning Application:** Demonstrated the application of deep learning techniques (autoencoders and LSTMs) for IoT intrusion detection, highlighting their efficacy in handling complex network traffic patterns.

**Performance Visualization:** Used plots and metrics such as accuracy and loss curves, along with classification reports, to showcase model effectiveness and robustness.

**Future Directions:**

**Enhanced Model Architectures:** Explore more sophisticated deep learning architectures (e.g., attention mechanisms) to further improve detection accuracy.

**Real-Time Implementation:** Transition models to real-time or edge computing environments for continuous monitoring and instant threat detection in IoT networks.

**Conclusion:** This project underscores the potential of deep learning in enhancing IoT network security through advanced intrusion detection systems. By leveraging LSTM networks and autoencoders, the project contributes to the advancement of cybersecurity solutions for IoT ecosystems, addressing critical challenges in network defense and resilience.
