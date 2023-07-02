# Question-Answering
The question answering is a Natural Language Processing(NLP) task, it has different approaches. In this project extractive question answering approach is used. It involves answering questions based on a given passage or document. In extractive QA, the answer is a span of text directly taken from the passage. The task requires understanding both the question and the passage, and selecting the most relevant information that correctly answers the question. 

Here's a step-by-step breakdown of how extractive QA works:

<b>Input:</b> The input to an extractive QA system consists of two main components:

<b>Question:</b> A natural language question that the system needs to answer.
Context: A passage or document containing the relevant information needed to answer the question.
Text Preprocessing: The question and context are preprocessed to remove any unnecessary noise, such as special characters or stopwords. This step also involves tokenizing the text into smaller units, such as words or subwords, to facilitate further analysis.

<b>Encoding:</b> The preprocessed question and context are converted into numerical representations that can be understood by machine learning models. This is typically done using techniques like word embeddings (e.g., Word2Vec, GloVe) or transformer-based models (e.g., BERT, GPT).

<b>Contextual Understanding:</b> The encoded question and context are fed into a model that can understand the relationship between the question and the passage. Transformer-based models, such as BERT or RoBERTa, are commonly used for this purpose. The model learns to encode the contextual information and capture the semantic meaning of the text.

<b>Answer Selection:</b> The model predicts the start and end positions of the answer span within the context. This is typically done using a combination of classification and token-level tagging techniques. The model assigns a probability to each token indicating whether it is the start or end of the answer span.

<b>Answer Extraction:</b> The tokens corresponding to the highest probabilities for the start and end positions are selected as the answer span. These tokens are then converted back into readable text to form the final answer.

<b>Post-processing:</b> The extracted answer may contain some extra words or lack coherence. Post-processing techniques like removing irrelevant words, merging fragments, or adding missing words can be applied to improve the answer's quality and readability.

<b>Evaluation:</b> The predicted answer is compared to a reference answer to evaluate its correctness. Metrics like exact match (EM) or token overlap, such as F1 score, are commonly used for evaluation.

Overall, extractive QA systems use machine learning models to understand and extract the most relevant information from a given context to answer questions accurately. These systems have various applications, including question answering on large document collections, customer support, or providing information retrieval from unstructured text sources.

