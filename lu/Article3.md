## Article (3) : Uncertainty Estimation and Quantification for LLMs: A Simple Supervised Approach (2024)
### Auteurs
Lia, et al.

### Lien
[Lire l’article]([https://drive.google.com/file/d/1DJmuUvLvFG8_ge9-4-gFXEZM51Rdgwg-/view?usp=drive_link](https://drive.google.com/file/d/1Od7v0-o7HfgTPBnsBJgm7-nsrUDRp4jb/view?usp=drive_link))

### Résumé
L’article propose une estimation supervisée de l’incertitude des LLM : on crée un jeu d’entraînement où chaque réponse est accompagnée d'une une mesure de qualité puis on apprend une régression qui prédit un score de confiance. Trois régimes sont étudiés : Wb‑S (accès aux activations internes ), Gb‑S (features probabilistes/entropie) et Bb‑S (modèle black box)


 <h3>Catégories des causes des hallucinations</h3>

Les causes sont regroupées en trois catégories : 

- **Données** (désinformation, biais, lacunes de connaissances)
- **Entraînement** (pré‑entraînement, fine‑tuning supervisé, RLHF)
- **Inférence** (sur‑confiance, goulot d’étranglement du soft‑max, échec de raisonnement)

<h3>Techniques de detection </h3>

La detection s'appuie sur quatres axes :
- **Fact‑checking**
- **NLI**
- **Approches QA**
- **Métriques d’incertitude** : évaluées sur des bancs tels que **HalluEval**, **TruthfulQA** et **HalluQA**.
### Benchmarks spécifiques :

L'article répertorie les jeux de référence : HalluEval, Med‑HALT, TruthfulQA et décrit leurs domaines d’évaluation (ouvert, médical, factuel).

<p align="center">
  <img src="./uploads/figure1.PNG" width="500">
</p>
<h3>Techniques de mitigation </h3>

 Trois stratégies decrites :
- **Filtrage et amélioration des données**
- **Edition du modèle (knowledge editing, RLHF)**
- **RAG** (ou ses altérnatives)

<h3>Limitations du RAG et recommandations</h3>

L’article montre que le RAG échoue lorsque le récupérateur ne trouve pas de documents pertinents ou renvoie des sources contradictoires.

### Solutions proposées : 
- **Récupération adaptative**
- **Attribution robuste des sources**
- **Extension aux hallucinations vision‑langage et à la probing de la frontière de connaissance**

---

<h3> Conclusion </h3>
L'article formule explicitement des _open questions_ : comment mesurer la certitude du modèle, comment intégrer la supervision humaine à grande échelle, et comment concevoir des métriques universelles pour les deux niveaux de taxonomie.

---



