# Articles lus

Bienvenue dans le dossier `lu/` du repository **PFE Papers Summary**.  
Ce sous-dossier contient tous les articles que nous avons lus et résumés dans le cadre de notre PFE.

---

## Que trouve-t-on dans ce dossier ?
- L'ensemble des travaux et articles lus et résumés.
- pour chaque travail on trouve :
  - Le titre de l’article  
  - La référence ou le lien vers l’article  
  - Un résumé détaillé  
  - Les concepts clés  

---

## Article (1) : A Survey on Hallucination in Large Language Models: Definitions, Detection, and Mitigation (2026)

### Lien
[Lire l’article](https://www.preprints.org/frontend/manuscript/f9d1a7b519e1f4d5aa639cd7e0158fc0/download_pub)

### Résumé
L’article conclut que les hallucinations sont presque inévitables dans les modèles de génération probabiliste et que la voie la plus fiable consiste à intégrer l’estimation d’incertitude, la détection robuste et une supervision humaine dans une architecture en profondeur : données de haute qualité → alignement du modèle → contrôles d’inférence (RAG, auto‑vérification, interventions de décodage). 

 <h3>Principaux problèmes abordés</h3>
<p align="center">
  <img src="./uploads/tab1.PNG" width="500">
</p>

<h3>techniques de detection des hallucination/factualités</h3>
<p align="center">
  <img src="./uploads/tab2.PNG" width="500">
</p>

### Concepts clés (Défauts majeurs)

**Les fausses déclarations dans les LLMs s'organisent ainsi :**  

- **Hallucination (sortie qui contredit les connaissances accessibles du modèle)**
  
  - **Factualité vs. Fidélité** (dimension de l’exactitude externe vs. l’adhésion au contexte)

  - **Typologie principale**  
    - **Intrinsèque** : violation du contexte ou des instructions fournies (ex. chiffre d’affaires erroné)  
    - **Extrinsèque** : génération d’informations non vérifiables dans le contexte d’entraînement (ex. plans d’expansion inventés)
      
  - **Manifestations spécifiques**  
    - **Contradiction**  
      -> Factuelle (contre des faits connus)  
      -> Contextuelle (contre l’entrée fournie)  
    - **Fabrication** (entités, événements ou citations complètement inventés)  
    - **Sophisme logique** (raisonnement invalide, ex. « Si A > B et B > C, alors C > A »)  
    - **Incohérence d’instruction** (déviation par rapport à la consigne)  
    - **Incohérence de contexte** (déviation du texte source)  
    - **Erreur d’entité / de relation** (nom d’entité incorrect, relation déformée)  
---
