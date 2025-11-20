# Text-analysis-Project-for-mu-tinational-retail-brand
Sentiment and Topic Modeling analysis 
Customer Feedback Analysis – NLP, Sentiment Analysis & Topic Modeling
This project performs end-to-end text analytics on customer feedback data using Python.
It covers data preprocessing, sentiment analysis, topic modeling (NMF), and visualizations, and exports all outputs into Excel files & charts.
________________________________________
📁 Project Structure
├── Final GBA.xlsx                     # Raw dataset
├── preprocessed_data.xlsx             # After cleaning and preprocessing
├── sentiment_analysis_output.xlsx     # Sentiment scores & categories
├── topic_modeling_output.xlsx         # Discovered topics for each review
├── sentiment_pie_chart.png            # Sentiment distribution visualization
├── README.md                          # Project documentation
└── main_notebook.ipynb / script.py    # Your Python code
________________________________________
🚀 Key Features
1️⃣ Data Loading
•	Reads customer feedback Excel file using pandas.
•	Displays initial dataset structure.
2️⃣ Text Preprocessing
Performed using NLTK + Regex, including:
•	Lowercasing
•	Removing special characters
•	Tokenization
•	Stopword removal
•	Cleaning empty / missing data
This improves quality of text for sentiment & topic modeling.
3️⃣ Sentiment Analysis
Using TextBlob, the project:
•	Calculates polarity score
•	Assigns Positive / Negative / Neutral labels
•	Exports results → sentiment_analysis_output.xlsx
________________________________________
📈 Visualizations
✔ Sentiment Distribution Pie Chart
•	Colors:
o	Positive → Light Blue
o	Negative → Light Red
o	Neutral → Light Green
•	Saved as: sentiment_pie_chart.png
________________________________________
🧠 Topic Modeling (NMF)
Using TF-IDF Vectorizer + NMF, the model discovers hidden topics from feedback:
Example Output:
Topic 0: matches, perfectly, shipping, fast, description, product...
Topic 1: value, money, materialfinish, great, excellent...
Topic 2: amazing, service, packaging, recommend...
Topic 3: buy, loved, quick, delivery, quality...
Topic 4: exceeded, expectations, satisfied, product, size...
Each feedback row is assigned:
•	Topic_ID
•	Topic_Keywords
Saved into: topic_modeling_output.xlsx
✔ Topic Word Bar Charts
For each topic, a bar chart of top 10 words is generated.
________________________________________
🛠 Technologies & Libraries Used
Python Libraries
•	pandas
•	numpy
•	matplotlib
•	nltk
•	textblob
•	sklearn (TF-IDF & NMF)
•	re
•	ast
NLP Techniques
•	Tokenization
•	Stopword Removal
•	Sentiment Analysis
•	Topic Modeling (NMF)
•	TF-IDF Vectorization
________________________________________
📦 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/your-username/your-repo-name.git
2️⃣ Install Dependencies
pip install -r requirements.txt
If you don’t have a requirements.txt, here’s what to add:
pandas
numpy
nltk
textblob
scikit-learn
matplotlib
openpyxl
3️⃣ Download NLTK Data
Include once in your script:
import nltk
nltk.download('punkt')
nltk.download('stopwords')
________________________________________
▶ Running the Project
Option 1: Jupyter Notebook
Open:
jupyter notebook
Option 2: Python Script
python script.py
________________________________________
📂 Output Files Generated
File	Description
preprocessed_data.xlsx	Cleaned and tokenized text
sentiment_analysis_output.xlsx	With polarity & sentiment category
topic_modeling_output.xlsx	Topics for each review
sentiment_pie_chart.png	Sentiment distribution
topic_word_charts	Bar charts for each topic
________________________________________
📌 Future Improvements
•	Use VADER for more accurate sentiment on short reviews
•	Use LDA or BERTopic for deeper topic modeling
•	Create a complete web dashboard with Streamlit / Power BI
________________________________________
👩💻 Author
Vedika Upadhyay

