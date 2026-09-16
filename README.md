# Tableau des types de fautes — jeu de données

Ce dépôt contient une transcription structurée du PDF fourni par Samuel-Didier : « Tableau des types de fautes » (`2beb0857-0808-5c1a-b44f-dbeccf3ec35d`).

## Hiérarchie exacte du document

Le PDF est organisé comme un tableau à quatre niveaux de colonnes :

1. `categorie_id` / `categorie` : grande catégorie d'erreur.
2. `code` : code exact de la règle dans la catégorie.
3. `regle` : règle et formulation descriptive.
4. `exemples_incorrects` / `exemples_corrects` : exemples signalés par X et v dans le PDF.

Catégories présentes :

- `G` — Orthographe grammaticale : G1 à G6
- `P` — Ponctuation et typographie : P1 à P19
- `S` — Syntaxe : S1 à S12
- `U` — Orthographe d'usage : U1 à U3
- `V` — Vocabulaire : V1 à V7

Le code est donc distinct de la catégorie : par exemple `P` est le `categorie_id`, « Ponctuation et typographie » est le libellé de catégorie, et `P3` est le `code` de la règle concernée.

## Fichier principal

`guide_erreurs_grammaire.csv` est encodé en UTF-8 et utilise la virgule comme séparateur.

Colonnes :

- `categorie_id` : identifiant court exact de la catégorie (`G`, `P`, `S`, `U`, `V`).
- `categorie` : libellé de la catégorie.
- `code` : code exact de la règle (`G1`, `P1`, etc.).
- `regle` : texte de la règle.
- `explication` : description ou précision associée.
- `exemples_incorrects` : exemples fautifs, correspondant aux formes marquées X.
- `exemples_corrects` : corrections, correspondant aux formes marquées v.
- `source_pages` : pages du PDF utilisées.

Chaque ligne correspond à une règle du tableau source, et non à une catégorie indépendante.

## Source et fidélité

La structure a été vérifiée par analyse directe du PDF. Le PDF utilise les marqueurs X et v pour distinguer les formes fautives et corrigées. Les textes sont conservés autant que possible tels qu'extraits; les anomalies d'OCR ou les exemples présentés comme modèles plutôt que comme paires fautif/correct sont signalés dans les champs concernés.

Le fichier `guide_erreurs_grammaire_exemples_complets.csv` contient une sélection détaillée issue de l'analyse précédente; le fichier principal ci-dessus est désormais la référence unifiée et hiérarchique du dépôt.
