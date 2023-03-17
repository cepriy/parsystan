## Parsystan

# Description

This script is aimed at tagging aligned a bilingual text pair in a utf-8 encoded comma-delimited .csv file with pos_ner_xpos_deprel_head notation. I.e., each token of the text 
gets assigned underscored tags in the following order: token, pos, ner, xpos (treebank), dependency, head.
The tags are assigned as per [stanza](https://stanfordnlp.github.io/stanza/performance.html) library.

#Tagsets

[NER tags](https://github.com/stanfordnlp/stanza/issues/904)

[The POS tags are assigned as per UD](https://universaldependencies.org/u/pos/)

[Treebank specific POS tags (XPOS)](https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html)

[Dependency relation tags](https://universaldependencies.org/docs/u/dep/index.html)

#Installation

'Parsystan' runs on Python 3.8 or later.

Install the 'stanza' library:
```
pip install stanza  
```

#Usage

To run the script, execute the command:
```

python Parsystan.py <filename> <original_language_code> <translation_language_code>
```
The language codes are available [here](https://stanfordnlp.github.io/stanza/available_models.html).

The parsed file will be created in the same directory as the script.