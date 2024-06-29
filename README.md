# Inbox Guardian

This repostiory contains the code for Inbox Guardian, a framework to detect irrelevant and spam emails based on individual user preferences.

## File Structure:
- BERT Logs: A directory contianing logs of my hyperparameter tuning and results for the BERT encoder/decoder model.  
    - Binary Classification Log: A log of the hyperparameter tuning and overall results of BERT for the binary classification task.
    - Binary Graphs: Graphs of training and validation accuracy and loss when training the binary BERT classifier with the best hyperparameters
    - Trinary Classification Log: A log of the hyperparameter tuning and overall results of BERT for the trinary classification task.
    - Trinary Graphs: Graphs of training and validation accuracy and loss when training the trinary BERT classifier with the best hyperparameters
- Data: A directory containing a sample of the data I used for this project (I did not include the full dataset to protect the privacy of my emails)
- Experiments: A directory containing the code to train and evaluate the models I used
    - BERT_Encoder_Decoder: The code for the encoder/decoder model with BERT
    - Naive_Bayes: Code for Naive Bayes with both bag of words and Tf-Idf features
    - Random_Forest: Code for the random forest model
    - SGD_Classifier: Code for the logistic regression model and the SVM model
- Scraping: A directory that contains code related to scraping emails via the Gmail API
    - scrapeEmails: The code to generate the irrelevant/normal/urgent dataset for a Gmail user.  Note, this code relies on the user having "Unimportant," "Normal," and "Urgent" labels and populating them with the appropriate emails.  Also note that, in order to run, this code requires a user to log into their Gmail account and generate a credentials file and token.  I did not inlcude my versions of these files to protect my Gmail account.
- Guerrerio_J Write Up: A pdf copy of my final write-up
- requirements.txt: The library versions I used (for reproducability)
