# Question we are answering:
Mixtral 8x7B claims it is strong in French, German, Spanish and Italian.  What does this mean in terms of training, and does this mean other languages should be used in training to allow users in that language to use the advantages of AI?

### How we answered this:
We fine-tuned Mixtral on a question set in Hindi and Spanish to compare the results - and also did the same in RAG using an embeddings model from OpenAI and an evaluation model from RAG using a custom eval set in the native language, to see if the results were any different, but biased in the sense of that eval model.

### Results:
For RAG, 0% accuracy for Hindi, 50% accuracy for Spanish, English being a baseline that we presume is higher.  Finetuning results will be part of demo.

### Issues we encountered:
Internet issues, recent OpenAI model deprecations, the popularity of Mixtral on Hugging Face (kept timing out for RAG) and time for fine-tuning.  Also some great hallucinations in Hindi.

