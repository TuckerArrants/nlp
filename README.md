# NLP

A place to keep all of my natural language processing projects. Just as NLP is a rapidly growing field, so to is this repository. Currently, this repository contains notebooks and code that explores text classification, generation, and textual entailment using neural networks

# Table of Contents
1. Text Classification with Machine Learning
2. Textual Entailment with Transformers
3. Text Generation with GPT-2

# 1. Text Classification with Machine Learning
1. Used GloVe word embeddings and BiLSTMs\GRUs to classify tweets about natural disasters
2. Compared results to Google's BERT using the HuggingFace transformers library (over 84% f1-score for BERT 81% for BiLSTM/GRU blend)  
![](https://jalammar.github.io/images/BERT-language-modeling-masked-lm.png)

# 2. Textual Entailment with Transformers
1. Fine-tuned a multilingual RoBERTa (XLM-RoBERTa) with over 500 million parameters on TPUs, training over 12,000 samples in under 20 seconds an epoch
2. Experimented with NLP augmentation techniques by using Google translate to map sentences to random languages and back, generating additional samples to be used for training augmentation and test time augmentation
3. Accurately classified premise/hypothesis pairs for logical entailment in 15 different languages with an accuracy abover 80%
![](https://amitness.com/images/backtranslation-en-fr.png)

*Image from [@amitness](https://www.kaggle.com/amitness) on his excellent post on NLP augmentation [here](https://amitness.com/2020/05/data-augmentation-for-nlp/)*

# 3. Text Generation with GPT-2
1. Used OpenAI's GPT-2 model to generate text and tested different sampling techniques to improve coherence of produced text
Example: When fed the input: "Legolas and Gimli advanced on the orcs, raising their weapons with a harrowing war cry.", the generated output is: 
<blockquote>
Legolas and Gimli advanced on the orcs, raising their weapons with a harrowing war cry. A large, hairy orc with a long neck stood in their way, roaring in a powerful, guttural tongue. The hobbits cried out in alarm and hobbits-in-training shouted in relief. There was a pause as they considered the situation, then Gimli, Aragorn, and Legolas turned around to face the orc and began to run toward it.

"Aragorn!" yelled Gimli. "I want to know what is happening."

Aragorn took up the torch in his left hand and thrust it toward the orc. A massive axe appeared out of nowhere and smashed the orc's head...
                   
</blockquote>
