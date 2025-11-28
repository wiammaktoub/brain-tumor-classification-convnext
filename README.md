# Détection et Classification de Tumeurs Cérébrales par ConvNeXt

**Université Cadi Ayyad – Faculté des Sciences Semlalia, Marrakech**  
**Master ISI – Année 2025–2026**  
**Encadrant :** Pr. Mustapha AATILA  
**Réalisé par :** Maryem YMIL, Wiam MAKTOUB, Maryam BOUFOUS  

---

## Description
Ce projet utilise le **Transfer Learning** avec **ConvNeXt Tiny** pour classifier automatiquement les **tumeurs cérébrales** à partir d’images IRM en quatre catégories :  
- Glioma  
- Meningioma  
- Pituitary  
- No Tumor  

Le pipeline inclut le prétraitement des images (redimensionnement, normalisation, augmentation), le fine-tuning du modèle et l’évaluation via des métriques standards (Accuracy, Precision, Recall, F1-score, ROC-AUC).  

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

Le modèle est robuste et fournit des visualisations interprétables via Grad-CAM.

---

## Contenu du repository
- Dataset  
- notebooks Jupyter  
- Résultats et visualisations  
- Rapport final PDF   

---

## Lien GitHub
[https://github.com/wiammaktoub/brain-tumor-classification-convnext](https://github.com/wiammaktoub/brain-tumor-classification-convnext)

