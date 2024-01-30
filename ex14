import nltk
from nltk import CFG, ChartParser
grammar = CFG.fromstring("""
    S -> NP_SG VP_SG | NP_PL VP_PL
    NP_SG -> 'the' 'cat'
    NP_PL -> 'the' 'cats'
    VP_SG -> 'chases'
    VP_PL -> 'chase'
""")
parser = ChartParser(grammar)
def check_subject_verb_agreement(sentence):
    words = sentence.split()
    parse_trees = list(parser.parse(words))
    if not parse_trees:
        return "No valid parse tree found for the sentence."
    return "Subject and verb agree in the sentence."
sentences = [
    "the cat chases the cat",
    "the cats chase the cats",
    "the cat chases the cats",
    "the cats chase the cat",
]
for sentence in sentences:
    agreement_result = check_subject_verb_agreement(sentence)
    print(f"Sentence: {sentence}")
    print(f"Agreement: {agreement_result}")
    print()
