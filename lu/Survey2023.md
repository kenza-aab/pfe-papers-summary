
### Rawte, Sheth & Das (Septembre 2023)
### "A Survey of Hallucination in 'Large' Foundation Models"
## Référence complète : Rawte, V., Sheth, A., & Das, A. (2023). A Survey of Hallucination in “Large” Foundation Models.
# Type :
Narratif / Exploratoire.
# Objectif principal : 
Identifier et classifier les phénomènes d'hallucination à travers toutes les modalités des modèles de fondation (pas seulement le texte).
# Scope :
Multimodal (Texte, Image, Vidéo, Audio).
# Déf. hallucination : 
Contenu généré qui s'écarte de la réalité factuelle ou inclut des informations fabriquées.
# Autres concepts : 
*Fiabilité (Reliability)* et *Confiance (Trustworthiness)* (non définis formellement mais cités comme buts).
# Clarté des définitions : 
Moyenne. La définition reste très haut niveau pour englober les quatre modalités.
# Taxonomie : 
Basée sur la modalité de sortie.
# Texte : 
Hallucinations dans les LLMs.
# Image : 
Hallucination d'objets (présence d'objets inexistants).
# Vidéo / Audio :
incohérences temporelles ou sonores.
# Base de la taxonomie :
Modalité technique.
# Clarté / Complétude : 
Moyenne. Survole beaucoup de domaines sans entrer dans le détail des mécanismes internes du texte.
# Méthodes de détection :
- SelfCheckGPT (zéro-ressource, boîte noire).
- Analyses d'états internes (Internal State/SAPLMA).
- Évaluation des contradictions (Mündler et al.).
# Méthodes d'évaluation : 
Benchmarks comme HaluEval et Med-HALT.
# Métriques : 
Probabilité de token, entropie, score F1, exactitude (accuracy).
# Méthodes de mitigation :
- Alignement question-connaissance interactif.
- LLM-Augmenter (RAG + feedback automatisé).
- Chain-of-Knowledge (structuration de la connaissance externe).
# Contributions :
## Premier survey couvrant l'hallucination de manière multimodale.
