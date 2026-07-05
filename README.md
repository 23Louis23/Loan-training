# Loan Training App

App de suivi pour le Bloc 1 (Renfo, 4 semaines) du méga-cycle de Loan. Utilise la **même base de données Supabase** que Jox et Fifi (voir `Jox/jox-training-app/`) — pas besoin de recréer un compte ou un projet.

## Particularité par rapport aux autres apps

Le programme complet de Loan est un méga-cycle de 16 semaines en 4 blocs : Renfo (S1-S4) → Puissance (S5-S8) → Masse (S9-S12) → Force (S13-S16). Seul le Bloc 1 (Renfo) est digitalisé ici, car les exercices des blocs suivants n'ont pas encore été définis par le coach (comme prévu dans `Suivi_Charges_Loan.xlsx`, sheet "Planning Global"). Les charges de la semaine 1 déjà connues (extraites du suivi Excel) sont pré-remplies par défaut.

Quand le Bloc 2 (Puissance) sera prêt, donne les détails à Claude pour étendre `PROGRAMME` et `SEANCES` dans `index.html`.

## 1. Base de données

✅ Déjà faite — cette app utilise le même projet Supabase que Jox et Fifi, avec la colonne `athlete` qui sépare ses données des autres.

## 2. Configurer l'appli

✅ Déjà fait — `index.html` contient l'URL et la clé Supabase, et un code d'accès (`7531` par défaut, modifiable en cherchant `APP_PIN` dans le fichier).

## 3. Déployer sur Vercel (gratuit) — sans rien installer

Même procédure que pour Jox et Fifi :

1. Crée un nouveau repo GitHub (ex: `loan-training-app`).
2. Sur la page du repo vide, clique **"uploading an existing file"**, glisse-dépose `index.html` et `README.md`, **Commit changes**.
3. Va sur [vercel.com/new](https://vercel.com/new), **Import** le repo `loan-training-app`, laisse les réglages par défaut, **Deploy**.
4. Récupère l'URL propre du projet (section "Domains", sans caractères aléatoires).

## 4. Utilisation

Envoie l'URL + le code `7531` à Loan. Toi, tu ouvres la même URL sur ton ordinateur avec le même code pour suivre ses séances et sa progression.
