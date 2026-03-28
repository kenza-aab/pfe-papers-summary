## Article (3) : Uncertainty Estimation and Quantification for LLMs: A Simple Supervised Approach (2024)
### Auteurs
Liu, et al.

### Lien
[Lire l’article](https://drive.google.com/file/d/1Od7v0-o7HfgTPBnsBJgm7-nsrUDRp4jb/view?usp=sharing)

### Résumé
L’article propose une estimation supervisée de l’incertitude des LLM : on crée un jeu d’entraînement où chaque réponse est accompagnée d'une une mesure de qualité puis on apprend une régression qui prédit un score de confiance. Trois régimes sont étudiés : Wb‑S ( **white-box** accès aux activations internes ), Gb‑S (**Grey-box** features probabilistes/entropie) et Bb‑S (**black box**)

**Approche supervisée** : première formalisation du problème d’incertitude comme régression à partir de réponses labellisées, alors que les enquêtes se concentrent sur des métriques non‑supervisées ou des détecteurs heuristiques


 <h3>Points clés</h3>

 - Les expériences montrent que les modèles supervisés surpassent les baselines non‑supervisées et améliorent la calibration, même en out‑of‑distribution QA
 - **Utilisation des activations cachées** : démonstration que les neurones internes contiennent de l’information d’incertitude, exploitée uniquement dans le mode white‑box
 - Applicabilité aux modèles fermés : le régime black‑box (Bb‑S) permet d’estimer l’incertitude d’un LLM propriétaire en utilisant un "LLM tool" ouvert
 - les activations internes du modèle (états cachés) contiennent un signal d’incertitude suffisamment puissant pour être appris par une régression supervisée, ce qui permet de prédire un score de confiance directement corrélé aux hallucinations. Cette approche « white‑box » montre que, contrairement aux travaux antérieurs qui se limitaient à des métriques de sortie (logits, entropie) ou à des méthodes non‑supervisées, on peut exploiter les représentations internes du LLM pour détecter et quantifier les hallucinations de façon plus précise et calibrée

---
### L'idée
Pour toute question donnée (input) le LLM genère une réponse(output). Le but de l'estimation de l'incertitude est de créer un système capable de prédire la qualité de cette réponse. 
On peut distinguer trois pilliers de qualité: 
- La confiance : assurance interne du modèle est ce que les propbabilités mathématiques sont elevées ?.
- La vérité : c'est l'adéquation avec le monde réel. 
- L'incertitude : La mesure du doute. 

---
### Notion de calibration 
c'est l'adéquation entre la confiance affiché par un modèle et sa précision réelle ... to be continued.

### Activation de neurones cachés 

Le point de rupture de ce papier est le passage d'une analyse de surface (probabilités des tokens) à une analyse structurelle (**activations des neurones cachés**).

**Pourquoi c'est important :**
1. **Richesse de l'information :** Les activations contiennent des dimensions d'incertitude invisibles dans l'output final.
2. **Indépendance du modèle :** En utilisant un "Tool LLM", on peut quantifier l'incertitude de n'importe quel modèle propriétaire (GPT-4, Claude) sans accès à ses poids.
3. **Supervision simple :** Transformer l'incertitude en une tâche de régression supervisée rend le système beaucoup plus robuste face aux hallucinations.




