
## Zhang et al. (2025)
# "Siren’s Song in the AI Ocean: A Survey on Hallucination in Large Language Models"
## Référence complète : Zhang, Y., Li, Y., Cui, L., et al. (2025). Siren’s Song in the AI Ocean: A Survey on Hallucination in Large Language Models.
### Type : Systématique et thématique.
### Objectif : Recenser les efforts sur la détection, l'explication et l'atténuation des hallucinations, avec un accent sur les défis spécifiques aux LLMs.
### Scope : 
Général (LLMs textuels).
### Déf. hallucination : 
Contenu généré divergeant de l'entrée utilisateur, contredisant le contexte généré précédemment ou s'écartant de la connaissance mondiale établie.
### Concepts liés :
- #### Factuality : Cohérence avec les faits mondiaux.
- #### Faithfulness : Fidélité à la source fournie.
### Taxonomie : basée sur le Conflit.
- Input-conflicting : Déviation par rapport à l'instruction ou au texte source.
- Context-conflicting : Auto-contradiction au sein d'une longue génération.
- Fact-conflicting : Incohérence avec la connaissance mondiale (inclut le contenu invérifiable).
### Base de la taxonomie : Source du conflit/incohérence.
### Clarté / Complétude : 
Bonne / Élevée.
### Détection :
- Modèle comme juge : GPT-Judge.
### Heuristiques : BLEU, ROUGE, entités nommées.
### Analyse de probabilité : Log-probabilités de séquence.
### Mitigation : Classée par Cycle de vie du LLM :
- Pré-entraînement : Curation et filtrage de données massives.
- SFT (Fine-tuning supervisé) : Intégration d'échantillons d'honnêteté ("Je ne sais pas").
- RLHF : Récompenses axées sur l'honnêteté (Honesty-oriented RL).
### Inférence : Stratégies de décodage (Factual-nucleus sampling, COVE), RAG, analyse d'incertitude.

---

### Pertinence : Forte.
