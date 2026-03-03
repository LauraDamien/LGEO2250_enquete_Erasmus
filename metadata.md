# Métadonnées du jeu de données

## 1. Identification du jeu de données

Titre : Erasmus Destination Preference Survey – Belgique (2026)

Créateurs :
- Lucas Wautot
- Nicolas Jamar Rodriguez
- Eléonore Vanderlinden
- Laura Damien

Date de création du jeu de données : 27/02/2026  
Langue des données : Français  
Type de ressource : Jeu de données d’enquête  
Version : 1.0  

---

## 2. Description du contenu

Jeu de données anonymisé (N = 170) issu d’une enquête en ligne portant sur :

- L’intention de partir en mobilité académique (Erasmus)
- Les préférences régionales de destination
- Les caractéristiques socio-académiques des répondants
- Les facteurs influençant la décision (échelles de Likert)
- Les destinations idéales mentionnées en réponse ouverte

---

## 3. Méthodologie de collecte

Méthode : Questionnaire en ligne (Microsoft Forms)  
Stratégie d’échantillonnage : Échantillon de convenance  
Période de collecte : 16/02/2026 – 27/02/2026  
Contexte géographique : Belgique (principalement Louvain-la-Neuve)

---

## 4. Structure des fichiers

### Données brutes
Fichier : data_raw/enquete_erasmus_raw.xlsx  
Description : Export original de Microsoft Forms (non modifié)

### Données traitées
Fichier : data_processed/enquete_erasmus_clean.csv  
Format : CSV  
Encodage : UTF-8  
Séparateur : Virgule (,)  
Valeurs manquantes : NA

### Scripts
Langage : R  
Fonction : Nettoyage des données, analyses statistiques (Chi², Fisher), génération des figures

### Dictionnaire des variables
Fichier : metadata/data_dictionary.csv  
Contenu : nom de variable, type, modalités, description

---

## 5. Types de variables

- Variables nominales (genre, domaine d’étude, type d’habitat)
- Variables ordinales (échelles de Likert 1–5)
- Variables de classement (rang 1 à 10)
- Variables textuelles (réponses ouvertes)

---

## 6. Traitements effectués

- Suppression des réponses incomplètes
- Recodage de « Peut-être » en variable binaire pour certaines analyses
- Transformation des échelles de Likert en valeurs numériques (1 = Très peu → 5 = Très fort)
- Vérification des doublons
- Nettoyage des réponses ouvertes

L’ensemble des étapes est reproductible via les scripts du dossier `/scripts`.

---

## 7. Interopérabilité

Formats ouverts utilisés :
- CSV
- Scripts R (.R)

Logiciels compatibles :
- R
- Python
- SPSS
- Excel
- QGIS

---

## 8. Sensibilité et protection des données

- Aucune donnée personnelle identifiable
- Jeu de données entièrement anonymisé
- Conforme aux principes du RGPD

---

## 9. Réutilisation

Les données sont :

- Structurées
- Documentées
- Fournies avec dictionnaire de variables
- Accompagnées d’un workflow reproductible

---

## 10. Licence

MIT License

---

## 11. Provenance scientifique

Jeu de données créé dans le cadre du cours LGEO2250 – Mesures de terrain en Géographie (UCLouvain, 2025–2026).

Les données ont été collectées, nettoyées et analysées par des étudiants en Master en sciences géographiques dans un objectif pédagogique.

Les analyses statistiques ont été réalisées sous R (version 4.x).