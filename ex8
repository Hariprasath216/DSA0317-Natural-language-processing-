import random
sentence = "The quick brown fox jumps over the lazy dog"
words = sentence.split()
pos_model = {
    'The': 'DT',
    'quick': 'JJ',
    'brown': 'JJ',
    'fox': 'NN',
    'jumps': 'VB',
    'over': 'IN',
    'the': 'DT',
    'lazy': 'JJ',
    'dog': 'NN'
}
pos_tags = [pos_model.get(word, random.choice(['NN', 'VB', 'JJ', 'DT', 'IN'])) for word in words]
tagged_sentence = list(zip(words, pos_tags))
print(tagged_sentence)
