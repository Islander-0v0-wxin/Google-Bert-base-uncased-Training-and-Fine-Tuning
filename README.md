The base model is google/bert base uncased model, trained and fine-tuned on a balanced dataset, consisted of 5.23k human-written text originated from IMDB movie reviews and 5.23k LLM-generated Text (The dataset can be found at: https://huggingface.co/datasets/Milkyway-islander/AI_Human_generated_movie_reviews). 
In order to customize the model specifically for a binary classification task, we train the dense layer with activation = "sigmoid" and "loss function = binarycrossentrophy". More details can be found inside the code. 

References: https://towardsdatascience.com/hugging-face-transformers-fine-tuning-distilbert-for-binary-classification-tasks-490f1d192379
