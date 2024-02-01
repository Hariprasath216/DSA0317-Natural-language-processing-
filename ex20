import nltk
from nltk.corpus import wordnet
from nltk.wsd import lesk
nltk.download('wordnet')
sentence = "I saw a bat flying in the cave."
word = "bat"
tokens = nltk.word_tokenize(sentence)
sense = lesk(tokens, word)
if sense:
    print("Word:", word)
    print("Sense:", sense.name())
    print("Definition:", sense.definition())
    print("Examples:", sense.examples())
else:
    print("No suitable sense found for the word.")
