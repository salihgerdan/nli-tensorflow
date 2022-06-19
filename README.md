# nli-tensorflow
Natural Language Inference using bidirectional LSTMs

The problem of natural language inference is important for many other sub-tasks in NLP.
It aims to determine the entailment relationship between two natural language sentences.

This project implements the neural model proposed by Rocktäschel et al. (2015) to solve this
problem. It is an LSTM based model that reads both sentences, instead of encoding the
sentences separately.

### Some examples of the task
"A man inspects the uniform of a figure in some East Asian country."
**contradicts** with
"The man is sleeping"

"A soccer game with multiple males playing."
**entails**
"Some men are playing a sport."

"A person on a horse jumps over a broken down airplane."
is **neutral** with
"A person is training his horse for a competition."

### Results
The resulting system achieved 72% accuracy on the Stanford NLI dataset.

You can read the attached [paper](paper.pdf) for explanation and
find the Jupyter Notebook [file](project.ipynb) for the implementation.

#### Reference
Rocktäschel, T., Grefenstette, E., Hermann, K. M., Kočiský, T., & Blunsom, P. (2015). Reasoning about
entailment with neural attention. arXiv preprint arXiv:1509.06664.
