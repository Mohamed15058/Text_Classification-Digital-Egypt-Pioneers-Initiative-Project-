# 📝  Text_Classification (Digital-Egypt-Pioneers-Initiative-Project)
This project demonstrates how to deploy a machine learning text classification model using Flask. The model classifies BBC news headlines into categories like business, politics, sports, tech, and entertainment.

# 📋 Table of Contents   
📝 Text Classification with Flask      
  📋 Table of Contents    
  🗂️ Project Structure    
  🚀 Getting Started    
    🔧 Prerequisites     
   📦 Installation and Setup   
      For Mac and Linux Users   
      For Windows Users     
   💻 Running the Application    
       Running Locally   
   📚 API Documentation       
# 🗂️ Project Structure   
Digital-Egypt-Pioneers-Initiative-Project/   
├── models/   
│   └── text_classification_model.h5 # Trained text classification model     
├   └── tokenizer.pickle             # Serialized tokenizer for text preprocessing   
├── templates/   
│   ├── index.html               # Main form for input and prediction  
├── bbc-text.csv                 # Dataset for training and prediction   
├── app.py                       # Flask app handling model inference   
├── requirements.txt             # Python dependencies   

# 🚀 Getting Started    
# 🔧 Prerequisites    
To run this project, you will need:   

  *Python 3.x installed on your system   
  *Flask (for the web app)   
  *TensorFlow (for loading the pre-trained model)   
  * NLTK (for text preprocessing)    
Wordcloud (for generating wordclouds)  
# 📦 Installation and Setup   
For Mac and Linux Users   
1- Clone the repository:         
 git clone https://github.com/yourusername/Digital-Egypt-Pioneers-Initiative-Projectgit   
 cd Digital-Egypt-Pioneers-Initiative-Project      
2-Create a virtual environment:
python3 -m venv venv
source venv/bin/activate     
3-Install the dependencies:
pip install -r requirements.txt  
4-Run the application: 
python3 app.py   
5-Acess the web app:
http://localhost:5000    

For Windows Users
1-Download the requirements.txt file
2-Create a virtual environment:
python -m venv venv
source venv/Scripts/activate    
3-Install the dependencies:
pip install -r requirements.txt
4-Run the application:
python app.py
5-Acess the web app:
http://localhost:5000  


