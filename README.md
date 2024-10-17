# ELIta
Emotion Lexicon for Italian

![Copia di Copia di ELIta (2)](https://github.com/user-attachments/assets/6d315572-744c-46fc-9264-47b0dfd0a0f1)

The lexicon comprises 6905 items, including both words and emojis. The data set contains 21 % adjectives, 50 % of nouns, 21 % verbs and 8 % of words that can beconsidered both as adjective and noun. In addition, a smaller number of adverbs, expressions (e.g. ‘restare a bocca aperta’ be looking open-mouthed) and interjections (e.g. ‘beh’, ‘boh’) have been included. the data collection involved an annotation process that included both the association of words with basic emotions (Plutchik' Wheel of Emotions), using a scale
from “non associated” (0), “weakly associated” (0.25), “moderately associated” (0.75) to “strongly associated” (1), and the evaluation of the items according to VAD dimensions (valence, arousal and dominance) using a 1 to 9 scale. Each of the 6905 words/emojis in the lexicon has got from a minimum of 5 annotations to a maximum of 10 annotations (on average 5.13 annotations per word).

The lexicon is provided in several versions: 

# RAW Version 
including all annotations and demographic metadata with an average inter-annotator agreement (calculated with Krippendorff) of 0.67. The csv file presents the word/emoji, age and gender columns of the annotator, the basic emotions with annotations from 0 to 1 and the emotion dimensions from 1 to 9

# GOLDEN version 

A second, non-aggregated version was also released, in which the five most similar annotations were selected for words with more than five annotations, thereby excluding the outliers. Additionally, an automatically generated ’golden standard’ annotation was added for each word, calculated based on the majority vote from the five annotations for each emotion. This approach emphasizes the majority vote while retaining all individual entries. This ’ELIta-golden’ version achieves an Inter- Annotator Agreement (IAA) of 0.874. The annotations are categorized by origin into ’ELIta,’ ’ELIta-selected’ for selections made from more than five annotations, and ’golden.’ In this case, demographic information is absent, but association intensity is preserved. The csv file presents the word columns, the origin of the annotation (elita or golden), the basic emotions with annotations from 0 to 1 and the emotion dimensions from 1 to 9.

# INTENSITY 

One of the aggregate versions created from the golden version retains the intensity values of the original annotations, with the single value calculated as the average of the six annotations (five original + one golden). The decision to use the golden version is to balance the few annotations with one representative of the majority. In this case, the labels of love automatically calculated from the values of joy and trust and ‘neutral’ were also added. The txt file presents the columns word/emoji, emotion or dimension and the association intensity from 0 to 1 (for basic emotions and Love) or 1 to 9 for the dimensions. 

# BINARY 

The second aggregated version, converts the aggregated float values to integers, providing a binary representation of the basic emotions: 0 for values below 0.50 and 1 for values above 0.50. The txt file presents the word, emotion or dimension column, and the presence (1) or absence of the emotion (0) or the emotion dimension ratings from 1 to 9.

- The lexicon is the result of a doctoral thesis project in Linguistics carried out at the Department of Letters and Modern Cultures at Sapienza University of Rome in collaboration with Roma Tre.
