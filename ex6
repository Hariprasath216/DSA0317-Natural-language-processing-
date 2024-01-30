import random
sample_text = "This is a sample text "
words = sample_text.split()
bigrams = [(words[i], words[i+1]) for i in range(len(words)- 1)]
generated_text = []
current_word = random.choice(words)  
for _ in range(50):  # Generating 50 words
    next_candidates = [b[1] for b in bigrams if b[0] == current_word]
    if next_candidates:
        next_word = random.choice(next_candidates)
    else:
        next_word = random.choice(words)  
    generated_text.append(current_word)
    current_word = next_word
generated_text = ' '.join(generated_text)
print("\n",generated_text)
