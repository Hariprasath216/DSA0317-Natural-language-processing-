import re
sentence = "The quick brown fox jumps over the lazy dog"
pos_rules = [
    (r'\bThe\b', 'DT'),             # Determiner
    (r'\bquick\b', 'JJ'),           # Adjective
    (r'\bbrown\b', 'JJ'),           # Adjective
    (r'\bfox\b', 'NN'),             # Noun
    (r'\bjumps\b', 'VB'),           # Verb
    (r'\bover\b', 'IN'),            # Preposition
    (r'\bthe\b', 'DT'),             # Determiner
    (r'\blazy\b', 'JJ'),            # Adjective
    (r'\bdog\b', 'NN')              # Noun
]
words = sentence.split()
pos_tags = []
for word in words:
    for pattern, pos_tag in pos_rules:
        if re.search(pattern, word, re.IGNORECASE):
            pos_tags.append((word, pos_tag))
            break
    else:
        pos_tags.append((word, 'NN'))  
print(pos_tags)
