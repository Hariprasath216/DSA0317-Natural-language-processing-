from nltk import PorterStemmer
from nltk.tokenize import word_tokenize
import nltk
nltk.download('punkt')
nltk.download('wordnet')
nltk.download('words')
nltk.download('stopwords')
nltk.download('maxent_ne_chunker')
text="you must be takecare  while crossing road and also lookup the magically"
port= PorterStemmer()
words=word_tokenize(text)
print(words)
stem1=[port.stem(word) for word in words]
print(stem1)
