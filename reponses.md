# 📝 Réponses TP3 - Branches et Fusion

## 📌 Exercice 1 : Création et navigation entre branches

### 🔹 1. Création des branches et navigation
Commandes utilisées :
```bash
git branch feature-1
git branch feature-2
git branch  # Liste des branches
git checkout feature-1
echo "Modification dans feature-1" >> README.md
git add README.md
git commit -m "Modification dans feature-1"
git checkout main

exo 2
git branch dev
git checkout dev
echo "Ceci est un fichier de notes." > notes.txt
git add notes.txt
git commit -m "Ajout du fichier notes.txt"
git checkout main
git merge dev
exo3
git branch conflit-test
git checkout main
echo "# Projet d'exercice - Version Main" > README.md
git add README.md
git commit -m "Mise à jour du README dans main"
git checkout conflit-test
echo "# Projet d'exercice - Version Test" > README.md
git add README.md
git commit -m "Mise à jour du README dans conflit-test"
git checkout main
git merge conflit-test
exo4
git branch feature-rebase
git checkout feature-rebase
echo "Ceci est un fichier feature." > feature.txt
git add feature.txt
git commit -m "Ajout du fichier feature.txt"
exo 5
git branch feature-a
git branch feature-b
git branch feature-c
git checkout feature-a
echo "Feature A" > feature-a.txt
git add feature-a.txt
git commit -m "Ajout de feature-a.txt"

git checkout feature-b
echo "Feature B" > feature-b.txt
git add feature-b.txt
git commit -m "Ajout de feature-b.txt"

git checkout feature-c
echo "Feature C" > feature-c.txt
git add feature-c.txt
git commit -m "Ajout de feature-c.txt"
exo6
git add reponses.md
git commit -m "Solution TP3"
git remote add origin <URL_DE_VOTRE_DEPOT>
git push origin HEAD --force
git push origin conflit-test
git push origin feature-rebase
git push origin feature-a
git push origin feature-b
git push origin feature-c
