
In this notebook a transformer based NLP model is designed to automatically identify emotional states such 'happy', 'anger' that people express about a product on Twitter. Text classification is one of the most common tasks in NLP; it can be used for a broad range of applications, such as tagging customer feedback into categories or routing support tickets according to their language. So the approach discussed in the notebook can be extended to other application areas aswell.

### **The Transformer model used:**

we’ll tackle this task using a variant of BERT called [DistilBERT](https://huggingface.co/docs/transformers/model_doc/distilbert). The main advantage of this model is that it achieves comparable performance to BERT, while being significantly smaller and more efficient

### **The Dataset:**

To build our emotion detector I have used a great dataset from an [article](https://aclanthology.org/D18-1404/) that explored how emotions are represented in English Twitter messages. Unlike most sentiment
analysis datasets that involve just “positive” and “negative” polarities, this dataset contains six basic emotions: anger, disgust, fear, joy, sadness, and surprise. Given a tweet, our task will be to train a model that can classify it into one of these emotions.
