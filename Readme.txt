

 Parallel Computing in Julia: Hyperspectral Image Unmixing

 Description
Ce projet explore l'utilisation de la parallélisation en Julia pour résoudre un problème d’unmixing d’images hyperspectrales. Le but est de développer un algorithme efficace capable d’extraire les signatures spectrales (endmembers) et leurs proportions relatives (abundance) dans les pixels d'une image hyperspectrale. Le projet met l’accent sur l’optimisation des performances par la parallélisation sur plusieurs cœurs de processeur.

---

 Objectifs
1. Implémenter l’algorithme d’unmixing spectral :  
   - Résoudre un problème d’optimisation avec des contraintes :
     - Non-negativité des proportions (ANC).
     - Somme des proportions égale à 1 (ASC).
2. Visualiser et interpréter les résultats pour valider les performances.
3. Développer une version parallélisée de l’algorithme en :
   - Utilisant une parallélisation pixel-par-pixel ou par sections d’image.
   - Comparant les versions séquentielles et parallélisées.
4. Étudier les temps d’exécution en fonction de :
   - La taille de l’image en entrée.
   - Le nombre de processus utilisés.
   - Les critères d’arrêt de l’algorithme.

---

 Méthodologie
- Modèle linéaire de mélange spectral (LMM) :
  -  X = SA + E 
  -  X  : matrice des données (pixels).
  -  S  : signatures spectrales (endmembers).
  -  A  : proportions des endmembers (abundance).
  -  E  : bruit additif.
- Contraintes :
  - Non-négativité.
  - Somme égale à 1.
- Utilisation de l’algorithme de descente de gradient projetée pour résoudre les contraintes.

---

 Résultats attendus
- Gain de performance grâce à la parallélisation (réduction du temps d’exécution).
- Comparaison des approches séquentielles et parallélisées sur des images de différentes tailles.
- Validation des résultats grâce à des visualisations graphiques des signatures spectrales et des abondances.

---

 Configuration requise
- Julia v1.2 ou supérieur (v1.11 recommandé pour ses fonctionnalités avancées de parallélisation).
- Un ordinateur avec au moins 4 cœurs physiques pour des tests optimaux.

---

 Structure des fichiers
- `Project_parallelization_Julia_ABID_DAMMAK_SRIDI.ipynb` : Notebook Jupyter contenant l’implémentation et les résultats du projet.
- `julia_parallel_unmixing.pdf` : Documentation détaillée sur les objectifs et la méthodologie du projet.

---

 Instructions
1. Installez Julia (v1.2 ou supérieur) et les dépendances nécessaires.
2. Ouvrez le notebook Jupyter pour explorer le code et les résultats.
3. Testez le code sur des images d’entrée de différentes tailles pour évaluer les performances.

---

 Auteurs
- Iyed DAMMAK  
- ABID SRIDI  
- Lucas Drumetz (Superviseur, IMT Atlantique)

Pour toute question ou suggestion, n’hésitez pas à nous contacter.

---
