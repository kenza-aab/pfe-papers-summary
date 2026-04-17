## Huang et al. (Novembre 2023 - Janvier 2024)
# "A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions"
## Référence complète : Huang, L., et al. (2024). A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.
### Type : Systématique.
### Scope : Général (LLMs).
### Déf. hallucination : Contenu plausible mais non factuel.
### Concepts liés :
- Intrinsic Hallucination : Contredit la source.
- Extrinsic Hallucination : Invérifiable à partir de la source.
### Taxonomie : 
Distinction entre *Factuality Hallucination* (Entity-error, Relation-error) et *Faithfulness Hallucination* (Instruction/Context/Logical inconsistency).
### Base de la taxonomie : 
=> Nature de l'erreur (Vérité vs Fidélité).
### Détection :
Fact-checking (extraction et vérification de faits), estimation d'incertitude (via états internes ou comportement).
### Mitigation : 
Approches basées sur les Données (filtrage, édition de modèle), le Training (architectures bidirectionnelles comme BatGPT) et l'Inférence (décodage par contraste de couches comme DoLa).

---

### Point fort : 
Analyse très fine des causes (limites de l'attention, biais d'exposition, goulot d'étranglement softmax).
### Pertinence : Forte. Excellent pour détailler la partie "Causes techniques" du mémoire
