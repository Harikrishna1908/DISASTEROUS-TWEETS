# DISASTEROUS-TWEETS
      To predict which tweets are disasterous and which tweets are not using NLP and ML model
      
**3.1.	IMPORTING THE REQUIRED LIBRARIES:**

•	Libraries like  pandas , numpy are imported

•	Import libraries nltk – for tokenization;re – regular expression

•	From nltk we import PorterStemmer- for stemmerization

•	From sklearn wen import TfidfVectorizer- vectorizing the dataset using Tf – idf; imported train_test_split – split the train data;

•	SVC imported for creating ML model in SVM\

•	Imported accuracy score; confusion matrix; classification report using metrics from sklearn


**3.2.	TEXT PRE PROCESSING:**
•	The datasets for traning and testing are loaded to respective data frames created

•	Download the stop words and punkt from nltk

•	Stopwords are used to remove the words like ‘is’,’or’,etc.

•	cleaned_text_list = [] – created and a loop is created

•	in that the  URLS  & special characters are removed 

•	dataset are lowercased, tokenized , filtered and stemmerized

•	finally the text get append

•	in the similar way the datset also text processed

**3.3.	FEATURE EXTRACTION:**

•	Tfidf vectorizer is initialized

•	Taking fit_transform of the processed training datset we get the features of training data

•	Taking the transform of the processed test dataset we get the features of the test data

•	The train_test_split – split the features extracted from the train

•	X is dataframed as pre processed tex & y is dataframed as targets

**3.4.	ML MODEL BUILDING:**

•	We create  ML model to train the data

•	Here we are using SVM 

**3.5.	MODEL EVALUATION:**

•	Prediction of x_test  using svm model

•	Prediction of the features extracted from the test datset  using svm model

•	Accuracy, classification report tells about the accuracy of how much tweets can the ML model can detect

**3.6.	OUTPUT:**
•	sample['target'] = test_p: - load the predicted target values by the modelto the target of the sample 

•	sample.to_csv('submission.csv', index=False) – the sample is saved as csv  file in submission.csv
