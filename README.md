# Détection et Classification de Tumeurs Cérébrales par ConvNeXt

**Université Cadi Ayyad – Faculté des Sciences Semlalia, Marrakech**  
**Master ISI – Année 2025–2026**  
**Encadrant :** Pr. Mustapha AATILA  
**Réalisé par :** Maryem YMIL, Wiam MAKTOUB, Maryam BOUFOUS  

---

## Description du projet
Ce projet utilise le **Transfer Learning** avec **ConvNeXt Tiny** pour classifier automatiquement les **tumeurs cérébrales** à partir d’images IRM en quatre catégories :  
- Glioma  
- Meningioma  
- Pituitary  
- No Tumor  

Le pipeline inclut :  
- Prétraitement des images : redimensionnement, normalisation et augmentation.  
- Fine-tuning du modèle ConvNeXt Tiny.  
- Évaluation des performances avec **Accuracy**, **Precision**, **Recall**, **F1-score**, et **ROC-AUC**.  
- Visualisation interprétable des activations avec **Grad-CAM**.  

---

## Dataset
- Sources : Figshare, SARTAJ, Br35H  
- Total images : 7 023  
  - Training : 5 712  
  - Test : 1 311  

---

## Résultats
- Accuracy : 99,08 %  
- Précision, Recall, F1-score : ~0,991  
- ROC-AUC par classe : >0,999  

---

## Contenu du repository
- **Dataset** : dossiers Training et Testing  
- **Notebooks Jupyter** :  
  - `01_exploration.ipynb`  
  - `02_preprocessing.ipynb`  
  - `03_training.ipynb`  
  - `04_evaluation.ipynb`  
  - `05_gradcam.ipynb`  
- **Résultats et visualisations** : courbes, matrices de confusion, heatmaps  
- **requirements.txt** : bibliothèques Python utilisées  
- **Rapport final PDF**  

---

## Environnements utilisés

- **Machine distante (entraînement)** :
  - **GPU** : NVIDIA RTX 1000  
  - **CPU** : Intel(R) Xeon(R) w3-2423, 2112 MHz, 6 Cores, 12 Logical Processors  
  - **RAM** : 16 Go  
  - **OS** : Windows 11 Pro for Workstations  

- **Machine locale (développement)** :  
  Laptop personnel utilisé pour l’édition du code, le push Git et les visualisations  

---

## Installation et dépendances

1. **Cloner le projet depuis GitHub** :

```bash
git clone https://github.com/wiammaktoub/brain-tumor-classification-convnext.git
cd brain-tumor-classification-convnext
```

## Installation et exécution du projet
### Créer un environnement Conda

```bash
conda create -n brain-tumor python=3.11 -y
conda activate brain-tumor
```

## Installer les dépendances avec pip

```bash
pip install -r requirements.txt
```

## Exécution du projet
  - **Exploration des données**
   Ouvrir et exécuter 01_exploration.ipynb.
  - **Prétraitement des images**
   Ouvrir et exécuter 02_preprocessing.ipynb.
  - **Entraînement du modèle**
  Ouvrir et exécuter 03_training.ipynb.
  Le modèle entraîné sera sauvegardé dans results/training/best_convnext_model.pth.
  - **Évaluation du modèle**
  Ouvrir et exécuter 04_evaluation.ipynb.
  Les métriques et matrices de confusion seront générées dans results/evaluation/.
  - **Visualisation Grad-CAM**
  Ouvrir et exécuter 05_gradcam.ipynb.