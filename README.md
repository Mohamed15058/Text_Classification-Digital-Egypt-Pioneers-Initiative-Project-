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

# 💻 Running the Application
Running Locally
To run the application locally, you can run the following command:
python3 app.py    
# 📚 API Documentation
  ## Endpoint: /predict      
  * Method: POST        
  *Description: Accepts a news headline as input and predicts the category.   
# Request Example:
POST /predict
Content-Type: application/json

{
  "text": "ultimate game award doom sci-fi shooter doom blasted away competition major games ceremony golden joystick awards title win twice winning ultimate game year best pc game awards presented little britain star matt lucas much-anticipated sci-fi horror doom shot straight top uk games charts release august winners included grand theft auto san andreas took wanted christmas prize released last week closely followed halo half-life expected big hits unleashed later month missed prize wanted game went nintendo title legend zelda original doom released heralded new era computer games introduced graphics helped establish concept first-person shooter doom developed four years thought cost around top honour best online game year went battlefield vietnam chronicles riddick escape butcher bay handed unsung hero game release somewhat eclipsed doom released week however well received gamers praised storyline differed film released around time electronic arts named top publisher year taking crown nintendo annual awards voted readers computer video games magazines games awards like grown importance last six years uk market games grew worth record according recent report analysts screen digest"
}      
# Response Example:
{
  {
  "input_text": "ultimate game award doom sci-fi shooter doom blasted away competition major games ceremony golden joystick awards title win twice winning ultimate game year best pc game awards presented little britain star matt lucas much-anticipated sci-fi horror doom shot straight top uk games charts release august winners included grand theft auto san andreas took wanted christmas prize released last week closely followed halo half-life expected big hits unleashed later month missed prize wanted game went nintendo title legend zelda original doom released heralded new era computer games introduced graphics helped establish concept first-person shooter doom developed four years thought cost around top honour best online game year went battlefield vietnam chronicles riddick escape butcher bay handed unsung hero game release somewhat eclipsed doom released week however well received gamers praised storyline differed film released around time electronic arts named top publisher year taking crown nintendo annual awards voted readers computer video games magazines games awards like grown importance last six years uk market games grew worth record according recent report analysts screen digest",
  "predicted_category": "tech",
  "predicted_probability": 0.95
}
}


