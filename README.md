# DeepLearningNLP


|Item| BERT  | RoBERTa  | GPT-3
|--|--|--|--|
| Year | 2018  | 2019 | 2020
| Number of Parameters | 109M  | 125M | 175B
| Training Time | 12 days | 1 day | 34 days
| Infrastructure| 8x V100 GPUs | 1024 V100 GPUs | 10000 V100 GPUs
| Size of dataset used for training | 16GB | 160GB | 4500GB
| Training tokens (dataset) | 250B| 2000B | 300B
| Data source| Wikipedia |Wikipedia| Wikipedia
| | BookCorpus| BookCorpus | Common Crawl
| | | Common Crawl news dataset | WebText2
| | | OpenWebText | Books1
| | | Common Crwal stories| Books2


## Transfer Learning

 - Faster development 
 - Less data to fine-tune 
 - Good results

**Pre-training**

* Training a model from scracth
* Weights are randomly initialized
* Model is the pre-trained on large amounts of data


**Fine-Tuning**
Source Data -> ( Pre-training) -> Pretrained model -> (Fine-tuning)-> Fine-tuned model, NLP task-specific model

**Encoder-Decoder Model** BART, T5
Generative Tasks : Translation, Summarization

**Encoder-Only Model** BERT, RoBERTa, DistilBERT
Understanding of input: Sentence classification, Named entity recognition

**Decoder-Only Model** GPT, GPT-2, GPT-3
Generative Tasks

**Tasks BERT Does NOT Do**
Generate text
Text Translation
Text Summarization

**Tasks BERT Can Do**
Text Classification
Named Entity Recognition
Question Answering
Fill in the blank

**Subword Tokenization**
|  | BERT | GPT-2 / GPT-3
|--|--|--|
| Vocabulary size | 30522 | 50257
| Technique used | WordPiece| Byte-level , Byte-Pair Encoding,



**BERT (Bidirectional Encoder Representation from Transformers)**
**Self-Attention**
Inputs
 - Q ( Query)
 - K (Key)
 - V (Value)
