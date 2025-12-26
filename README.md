# Lab 4 - Deep Learning MBD : Auto-encoder, VAE et GANs

**Université Abdelmalek Essaâdi - Faculté des Sciences et Techniques de Tanger**  
**Département Génie Informatique**  
**Master MBD - Deep Learning**  
**Professeur : Pr. ELAACHAK LOTFI**

---

## Objectif du laboratoire
Se familiariser avec la bibliothèque **PyTorch** pour construire et entraîner des modèles génératifs :
- Auto-encoder (AE)
- Variational Auto-encoder (VAE)
- Generative Adversarial Networks (GANs - DCGAN)

---

## Travail réalisé

### Partie 1 : AE et VAE (dataset MNIST)
- Implémentation d’un Auto-encoder classique et d’un Variational Auto-encoder
- Entraînement sur MNIST avec les hyper-paramètres suivants :
  - Dimension latente : 10
  - Learning rate : 0.001
  - Batch size : 128
  - Nombre d’époques : 20
  - Optimiseur : Adam
- Évaluation : courbes de loss (reconstruction + KL pour VAE)
- Visualisation de l’espace latent des deux modèles avec t-SNE
- Conclusion : Le VAE produit un espace latent plus continu et structuré grâce à la régularisation KL, idéal pour la génération.

### Partie 2 : GANs (dataset Abstract Art Gallery)
- Implémentation d’un DCGAN (Generator et Discriminator convolutionnels)
- Hyper-paramètres :
  - Dimension du bruit z : 100
  - Learning rate : 0.0002
  - Batch size : 64
  - Nombre d’époques : 50
  - Optimiseur : Adam (betas=(0.5, 0.999))
- Évaluation : courbes de loss du Generator et du Discriminator
- Génération de nouvelles images et comparaison visuelle avec les originales
- Conclusion : Le modèle génère des images abstraites capturant le style (couleurs, formes) du dataset original.

---

## Synthèse : Ce que j'ai appris durant ce laboratoire

Ce TP m’a permis de consolider mes compétences en Deep Learning génératif avec PyTorch :
- Maîtrise complète de la construction de réseaux (MLP pour AE/VAE, convolutions transposées pour DCGAN)
- Compréhension approfondie des mécanismes : reconstruction (AE), reparametrization trick et KL divergence (VAE), entraînement antagoniste (GAN)
- Importance des hyper-paramètres, de la normalisation des données, et des bonnes pratiques (BatchNorm, LeakyReLU, initialisation des poids)
- Évaluation qualitative et quantitative des modèles génératifs (visualisation d’espaces latents, comparaison d’images)

Ce laboratoire constitue une excellente introduction pratique à la **Generative AI**.

---

**Fichier principal** : `Lab4_DeepLearning_AE_VAE_GAN.ipynb`  


**Auteur** : Wissal Choukri  
**Date** : 25 Décembre 2025

