# Chatbot-using-PyTorch

Data :
The Cornell Movie-Dialogs Corpus is a rich dataset of movie character dialog:
                  220,579 conversational exchanges between 10,292 pairs of movie characters
                  9,035 characters from 617 movies
                  304,713 total utterances
The data can be downloaded from https://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html.
This dataset is large and diverse, and there is a great variation of language formality, time periods, sentiment, etc.
   
   
 Model :
The brains of our chatbot is a sequence-to-sequence (seq2seq) model. The goal of a seq2seq model is to take a variable-length sequence as an input, and return a variable-length sequence as an output using a fixed-sized model.One RNN acts as an encoder, which encodes a variable length input sequence to a fixed-length context vector. In theory, this context vector (the final hidden layer of the RNN) will contain semantic information about the query sentence that is input to the bot. The second RNN is a decoder, which takes an input word and the context vector, and returns a guess for the next word in the sequence and a hidden state to use in the next iteration.
