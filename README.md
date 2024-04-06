# NLP-auto-spell-corrector-from-scratch
Spell Corrector
This repository contains a Python-based spell corrector developed from scratch. The spell corrector is designed specifically for English language and uses a Trie-based approach to efficiently find the closest correct spelling for any given word. It also implements a custom minimum edit distance algorithm where the substitution cost is 1 if the compared letters are adjacent on a QWERTY keyboard.

The English dictionary used in this project is obtained using the Natural Language Toolkit (NLTK), a leading platform for building Python programs to work with human language data.

Features
Efficient Spell Correction: The spell corrector can quickly find the most similar words in the dictionary for a given misspelled word.
Customizable: The spell corrector can be easily customized to work with any list of words.
Detailed Visualization: The spell corrector provides detailed visualization of the correction process, which can be helpful for debugging and understanding how the algorithm works.
Custom Minimum Edit Distance: The spell corrector implements a custom minimum edit distance algorithm that takes into account the QWERTY keyboard layout.
How it Works
The spell corrector uses a Trie data structure to store the dictionary of words. This allows for efficient prefix-based search to find similar words. The spell corrector then calculates the edit distance between the misspelled word and the similar words using a custom minimum edit distance algorithm. The words with the smallest edit distance are returned as the corrected words.

Usage
To use the spell corrector, simply create an instance of the SpellCorrector class and call the correct method with the misspelled word as the argument.

Python

corrector = SpellCorrector(dictionary)
corrected_words = corrector.correct(misspelled_word)
AI-generated code. Review and use carefully. More info on FAQ.
Future Work
Future improvements to the spell corrector could include support for weighted edit distance, where different types of edits (insertions, deletions, substitutions) have different costs. Additionally, the spell corrector could be extended to support multi-word correction, where the context of the word is taken into account when suggesting corrections.

Contributions
Contributions to the spell corrector are welcome. Please feel free to submit a pull request or open an issue on GitHub.
