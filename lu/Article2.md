## Article (2) : A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions (2024)

### Auteurs
Huang, et al.

### Lien
[Lire l’article](https://drive.google.com/file/d/1DJmuUvLvFG8_ge9-4-gFXEZM51Rdgwg-/view?usp=drive_link)

### Résumé
Huang et al. concluent que la taxonomie à deux niveaux pour classer les hallucinations des grands modèles de langage (hallucination factuelle (erreurs d’entité ou de relation) et hallucination de fidélité (non‑respect des instructions, incohérence contextuelle ou logique)) doit être alignée aux cas d’usage spécifiques et que les systèmes de récupération adaptative sont essentiel pour réduire les hallucinations dans les **IR** et LLMs. Ils appellent à une recherche continue sur les hallucinations vision‑langage afin de concevoir des défenses en profondeur combinant données, modèle et inférence.

 <h3>Catégories des causes des hallucinations</h3>

### Les causes sont regroupées en trois catégories : 

-**données** (désinformation, biais, lacunes de connaissances)
-**entraînement** (pré‑entraînement, fine‑tuning supervisé, RLHF)
-**inférence** (sur‑confiance, goulot d’étranglement du soft‑max, échec de raisonnement)

<h3>Techniques de detection </h3>

### La deection s'appuie sur quatres axes :
-**Fact‑checking**
-**NLI**
-**approches QA**
-**Métriques d’incertitude** : évaluées sur des bancs tels que **HalluEval**, **TruthfulQA** et **HalluQA**.

<h3>Techniques de mitigation </h3>

### Trois stratégies decrites :
-**Filtrage et amélioration des données**
-**Edition du modèle (knowledge editing, RLHF)**
-**RAG**

---


