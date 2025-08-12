Travel Interest Prediction – Decision Tree

Overview:
This project aims to predict users’ travel interests—such as Culture, Adventure, Beach, and Wildlife—based on their demographic profile and personal preferences. 
By leveraging a Decision Tree Classifier, the project transforms raw data into accurate predictions while offering interpretability and ease of use.
Encapsulated within a Flask web application, the model enables smooth interaction via a user-friendly interface.

Motivation:
In today’s world, offering personalized travel recommendations can significantly enhance user satisfaction and engagement.
This project demonstrates how machine learning can power such personalization, making otherwise complex tasks accessible and intuitive.
The Decision Tree model is especially fitting due to its straightforward logic, transparency, and ability to handle both numeric and categorical data effectively.

Dataset and Features:
The dataset, stored as Travel_Interest.csv, contains user profiles with the following key features:

Age
Gender
Preferred Activities (Hiking, Museums, Wildlife, etc.)
Budget Tier

Travel Frequency:
Inspired by real-world use cases, this data enables the model to learn meaningful patterns that underpin travel preferences.

Model Details:
A Decision Tree Classifier was chosen for its interpretability and efficiency. The model workflow includes:
Data Ingestion & Preprocessing: Loading the CSV, handling missing values (if any), encoding categorical features, and scaling numerical fields as needed.

Training: Fitting the Decision Tree to the preprocessed dataset, allowing the model to discover key decision splits.
Evaluation: Assessing performance using accuracy, precision, recall, and F1-score to ensure balanced and reliable predictions.
Serialization: Saving the model (travel_model.pkl) and necessary mapping files (destination_map.pkl, travel_type_map.pkl) for deployment.

Project Structure:
├── app.py                    
├── Train.py                  
├── Travel_Interest.csv       
├── travel_model.pkl          
├── destination_map.pkl       
├── travel_type_map.pkl      
├── templates/
│   └── index.html           
├── requirements.txt          
└── README.md                 

Results & Insights:
Early experiments show that the Decision Tree achieved strong classification performance, with accuracy in the range of X–Y% (please include your actual results).
Its interpretability also allows you to trace decisions—for example, whether budget or preferred activity was the decisive factor in a prediction—making it highly useful for analysis and optimization.

Future Enhancements:

In the future, this project can be enhanced by:
Expanding the dataset to include more diverse travel preferences and global demographics.
Integrating real-time user data from travel platforms to improve recommendation accuracy.
Adding hybrid models by combining Decision Trees with other algorithms like Random Forest or Gradient Boosting for better performance.
Personalized recommendations using NLP to analyze user reviews and feedback.
Mobile application integration for on-the-go travel interest predictions.
