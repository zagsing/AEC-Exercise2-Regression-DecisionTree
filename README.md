# Exercices AEC — Analyse d'affaires et analytique de données

## 📁 Contenu du projet

Ce dossier contient le corrigé complet des trois exercices avec code Python exécuté.

### Fichiers livrables

```
├── Corrige_Exercices.docx                      # Corrigé complet formaté (6 pages)
├── Exercice2_Regression_Detaille.ipynb         # Notebook : Régression linéaire (Q2.1-2.4)
├── Exercice3_Arbre_Decision_Detaille.ipynb    # Notebook : Arbre de décision (Q3.1-3.2)
├── Exercice2_Regression_Lineaire.ipynb         # Notebook initial (version brève)
├── Exercice3_Arbre_Decision.ipynb              # Notebook initial (version brève)
└── README.md                                    # Ce fichier
```

---

## 📊 Résumé des exercices

### **Exercice 1 : 
- 10 questions à choix multiples sur l'apprentissage automatique
- Réponses : Analyse en Composantes Principales, supervié/non-supervisé/renforcement, Classification, etc.
- Voir `Corrige_Exercices.docx`

### **Exercice 2 : Régression linéaire 

**Partie A — Cas de l'hôpital**
- Problématique : Patients qui quittent les urgences sans consultation (LWBS)
- Solution : Architecture multi-modèles (5 modèles chaînés)
- Modèles : Prévision affluence, Temps d'attente, Risque de départ, Segmentation, Facteurs explicatifs

**Partie B — Modèle de régression (Q2.1 à Q2.4)**
- Données : 12 étudiants (note intra → note finale)
- Q2.1 : Graphe + relation linéaire (r ≈ 0,78)
- Q2.2 : Critères MCO (minimiser SSE)
- Q2.3 : **Équation : ŷ = 32,03 + 0,58·x**
  - RMSE = 7,83 points
  - R² = 0,613 (61,3% variance expliquée)
- Q2.4 : Prédiction pour x=86 → **ŷ ≈ 82 points**

→ **Notebook détaillé** : `Exercice2_Regression_Detaille.ipynb`

### **Exercice 3 : Arbre de décision **

**Q3.1 — Modèle d'arbre**
- Données : 8 observations (AgeRange, Occupation, Gender → Happy)
- **Accuracy = 87,5 %** (7/8 correct)
- Note : 2 observations identiques (ID5, ID8) avec labels opposés → accuracy limitée
- Visualisation graphique de l'arbre incluse

**Q3.2 — Prédiction pour (young, professor, F)**
- Encodage one-hot + passage dans l'arbre
- **Résultat : Happy = No** (voir notebook pour détails)
- Probabilités affichées

→ **Notebook détaillé** : `Exercice3_Arbre_Decision_Detaille.ipynb`

---

## 🚀 Comment utiliser sur GitHub

### **Option 1 : Repository public simple**

1. **Créer un repo GitHub** : `AEC-Data-Analytics-Exercises`
2. **Cloner localement** :
   ```bash
   git clone https://github.com/[username]/AEC-Data-Analytics-Exercises.git
   cd AEC-Data-Analytics-Exercises
   ```
3. **Copier les fichiers** dans le dossier local
4. **Ajouter et pousser** :
   ```bash
   git add .
   git commit -m "Initial commit: Complete exercises with solutions"
   git push origin main
   ```

### **Option 2 : Avec structure organisée**

```
AEC-Data-Analytics-Exercises/
├── README.md
├── docs/
│   └── Corrige_Exercices.docx
├── exercice2_regression/
│   ├── Exercice2_Regression_Detaille.ipynb
│   └── Notes_Dataset.csv
├── exercice3_classification/
│   ├── Exercice3_Arbre_Decision_Detaille.ipynb
│   └── happiness_dataset.csv
└── .gitignore
```

### **Option 3 : Ajouter aux fichiers de projet existants**

Si vous avez déjà un repo pour votre AEC :
```bash
git add Exercices_AEC/*.ipynb Exercices_AEC/*.docx
git commit -m "Add complete exercise solutions with notebooks"
git push
```

---

## 📝 Points forts de ces livrables

✅ **Tous les résultats vérifiés** — Notebooks exécutés avec outputs visibles  
✅ **Équations et formules** — Mathématiques complètes en LaTeX  
✅ **Graphiques inclus** — Régression (scatter + droite) et arbre (visualisation)  
✅ **Code commenté** — Chaque étape expliquée en français  
✅ **Portfolio-ready** — Format professionnel, prêt pour les recruteurs  
✅ **Basé sur données réelles** — CSVs fournis (Notes_Dataset.csv, happiness_dataset.csv)  

---

## 🔧 Exécuter les notebooks localement

### Prérequis
```bash
pip install jupyter pandas numpy scikit-learn matplotlib
```

### Lancer Jupyter
```bash
jupyter notebook
```

### Exécuter les cellules
- **Une par une** : `Ctrl+Enter` (ou ⏵ Run)
- **Toutes à la fois** : Menu → Cell → Run All (ou `Ctrl+Alt+Enter`)

---

## 📚 Références et concepts couverts

| Exercice | Concepts | Méthodes |
|----------|----------|----------|
| 1 | ML paradigms, réduction dim., clustering, régularisation | QCM théorique |
| 2A | ETL, architecture, orchestration de modèles | Hôpital use-case |
| 2B | Régression linéaire, MCO, RMSE, R², prédiction | Scikit-learn |
| 3 | Decision tree, entropy, classification, accuracy | Sklearn + visualisation |

---

## 👤 Auteur

**AEC LEA.E2** — Zagre, Singapinda — Juin 2026

Travail présenté dans le cadre du programme **Analyse d'affaires et analytique de données**.

---

## 📄 Licence

Pour usage académique (portfolio, certification).

---

**Questions ou améliorations ?** N'hésitez pas à modifier et à enrichir ce projet ! 🚀
