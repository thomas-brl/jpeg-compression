# Compression JPEG

## Description

Ce projet consiste à implémenter une version simplifiée du format de compression d’images **JPEG**.

L’objectif est de simuler les principales étapes du traitement d’une image afin de comprendre le fonctionnement de la compression et de la reconstruction d’images numériques.

Les images utilisées sont représentées sous forme de tableaux **NumPy à 3 dimensions**, où chaque pixel est défini par un triplet RGB (Rouge, Vert, Bleu) avec des valeurs comprises entre 0 et 255.

---

## Objectif

Le but du projet est de :
- Manipuler des images sous forme matricielle
- Implémenter une version simplifiée du processus JPEG
- Tester la qualité de reconstruction des images

---

## Représentation des images

Une image est représentée par une matrice NumPy de dimensions :
(Hauteur, Largeur, 3)

Chaque pixel contient :
- Rouge (R)
- Vert (V)
- Bleu (B)

Chaque composante est un entier dans l’intervalle `[0, 255]`.

---

## Évaluation de la qualité

Pour comparer les images originales et reconstruites, nous utilisons le **PSNR (Peak Signal-to-Noise Ratio)**.

- PSNR = 100 → images identiques
- PSNR ≈ 40 → images très proches
- Plus le PSNR est élevé, meilleure est la qualité de reconstruction

---

## Fonctionnalités

- Chargement et affichage d’images
- Manipulation de matrices RGB
- Simulation simplifiée de compression JPEG
- Reconstruction d’image
- Mesure de similarité via PSNR

---

## Conclusion

Ce projet permet de comprendre les bases de la compression d’image JPEG à travers une implémentation simplifiée, en manipulant directement les pixels et en évaluant la qualité des reconstructions.
