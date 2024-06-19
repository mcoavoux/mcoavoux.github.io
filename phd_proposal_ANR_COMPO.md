#### Title: Structural Biases for Compositional Semantic Prediction

##### Scientific context

Compositionality is a foundational hypothesis in formal semantics and states that the semantic interpretation of an utterance is a function of its parts and how they are combined (i.e. their syntactic structure). In NLP, the current dominant paradigm is to design end-to-end models with no intermediate linguistically interpretable representations, which is often motivated by the fact that pretrained language models implicitly encode latent syntactical representations. However, recent studies suggest that the syntactic information learned by language models are insufficient and that, in their current form, they are unable to exploit the syntactic information provided in their input when they need to generate a structured output. 

Strikingly, most systems that obtained decent results on compositional generalization benchmarks either (i) include some data augmentation methods that increase the exposure of the model to diverse syntactic structures at training time, or (ii) resort to a natural language parser and hand-crafted rules to derive the semantic representation from the syntactic tree. These two approaches are efficient, but they still have limitations that need to be addressed. Firstly, data augmentation bypasses the issue altogether, is tied to a particular dataset or task and requires additional computation, both for generating new data and for re-training or fine-tuning models. Secondly, approach (ii) leaves the seq2seq framework for a more conceptually complex framework, and often uses architectures that are tied to specific data or tasks. In contrast, we believe that with proper built-in inductive biases, a seq2seq model might provide a simple, yet effective solution to the structural compositionality issue.

##### PhD Proposal

The goal of this PhD wil be to explore inductive biases related to linguistic structures, in an attempt to build small NLP models with compositional skills, i.e. models with built-in knowledge making them able to infer generalization rules from few data points. Research directions will be defined together with the successful applicant (who is encouraged to bring their own ideas!) and may include:

- Learning invariant language representations.  A risk of learning from little data or rare phenomena is that a model may rely on spurious correlations and be unable to generalize outside a specific context. Developing representations that are invariant to noise has been proposed as a way of improving generalization (Peyrard et al 2022). We propose to formalize invariants related to syntactic and semantic structures and explore ways to integrate them during the training phase.
- Syntactically constrained decoders. Unlike parsers, Seq2seq models are unable to generate structures unseen at train time. We propose to explore the use of structural constraints to guide decoding in seq2seq models.

Important information:

- Starting date:  between September and December 2024 (duration 3 years)
- Place of work: Laboratoire d’Informatique de Grenoble, CNRS, Grenoble, France
- Funding: ANR project ''COMPO: Inductive Biases for Compositionality-capable Deep Learning Models of Natural Language'’ (2024-2028)
- Partners: Université Paris Cité, Université Aix-Marseille, Université Grenoble Alpes
- The PhD will be supervised by Éric Gaussier and Maximin Coavoux, and in close collaborations with other partners  from the COMPO consortium, the PhD candidate will be part of 2 teams of the LIG: GETALP and APTIKAL.
- Salary: ~2300€ gross/month
- Profile: Master’s degree in NLP, computer science, experience in NLP and machine learning  

  To apply, please send cv, cover letter and most recent academic transcripts to eric.gaussier@univ-grenoble-alpes.fr and maximin.coavoux@univ-grenoble-alpes.fr

References:

SLOG: A Structural Generalization Benchmark for Semantic Parsing  
Bingzhi Li, Lucia Donatelli, Alexander Koller, Tal Linzen, Yuekun Yao, Najoung Kim  
<https://aclanthology.org/2023.emnlp-main.194/>

Structural generalization is hard for sequence-to-sequence models
Yuekun Yao, Alexander Koller
<https://aclanthology.org/2022.emnlp-main.337/>

Compositional Generalization Requires Compositional Parsers
Pia Weißenhorn, Yuekun Yao, Lucia Donatelli, Alexander Koller
<https://arxiv.org/abs/2202.11937>

Invariant Language Modeling  
Maxime Peyrard, Sarvjeet Ghotra, Martin Josifoski, Vidhan Agarwal, Barun Patra, Dean Carignan, Emre Kiciman, Saurabh Tiwary, Robert West  
<https://aclanthology.org/2022.emnlp-main.387/>
