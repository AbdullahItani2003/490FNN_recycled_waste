Plastic Waste Risk Classification Project

This project uses a feed-forward neural network to classify the risk level of coastal plastic waste for various countries based on plastic waste data. The neural network predicts whether the coastal waste risk is High, Medium, or Low based on features such as total plastic waste, recycling rate, and per capita waste.


Dataset

The dataset, Plastic Waste Around the World, includes the following columns:


Country: Name of the country

Total_Plastic_Waste_MT: Total plastic waste generated (in megatons)
Main_Sources: Main sources of plastic waste (e.g., packaging, consumer goods)
Recycling_Rate: Percentage of plastic waste that is recycled
Per_Capita_Waste_KG: Plastic waste per capita (in kilograms)
Coastal_Waste_Risk: The risk level of plastic waste affecting coastal areas (target variable)
The dataset is preprocessed by encoding categorical features and scaling numerical features for input into the neural network.


Model

The project utilizes a simple feed-forward neural network implemented with TensorFlow/Keras. The architecture includes:

Input Layer: Takes four features (scaled).
Hidden Layers: Two hidden layers with ReLU activation.
Output Layer: Three neurons with softmax activation for multi-class classification.
The model is compiled with categorical cross-entropy loss and optimized with the Adam optimizer.


Requirements

Python 3.x
TensorFlow
pandas
scikit-learn
