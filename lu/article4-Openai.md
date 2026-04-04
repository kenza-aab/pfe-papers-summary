# titre : Why language models hallucinate (2025)

## Selon l'article :

Les LLMs en produisant des fausses declarations flagrantes (hallucinations) deviennent pas très digne de confiance,
donc ou, durant la créations du modèle, a quel moment durant ce processus, ces hallucinations entrent-elles en jeu ?

- Distribution of language : Concept d'entraîner un LLM à partir d'un corpus d'entrainement,
  qui souvent et inévitablement, contient des erreurs et des half-truths. Selon l'article,
  même si on parviendrait à entrainer un LLM sur un dataset ayant 100% d'informations justes (ce qui n'est même pas possible);
  ce ne serait quand même pas suffisant pour eliminer totalement ou eviter que ce LLM hallucine !
  
  **The distribution of language is initially learned from a corpus of training examples, which
  inevitably contains errors and half-truths. However, we show that even if the training data were
  error-free, the objectives optimized during language model training would lead to errors being
  generated.** => the objectives optimized 🤔
