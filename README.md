# Guide des erreurs de grammaire — jeu de données

Jeu de données CSV extrait du PDF fourni par Samuel-Didier, intitulé « Tableau des types de fautes » (fichier source : Adobe Scan 16 sept. 2026.pdf). Le document couvre 47 entrées : 6 règles de grammaire (G1–G6), 19 règles de ponctuation/typographie (P1–P19), 12 règles de syntaxe (S1–S12), 3 règles d’orthographe d’usage (U1–U3) et 7 règles de vocabulaire (V1–V7).

## Fichier

`guide_erreurs_grammaire.csv`, encodage UTF-8, séparateur virgule.

Colonnes :
- `id` : identifiant de la règle dans le PDF.
- `categorie` : domaine linguistique.
- `titre` : intitulé de la règle.
- `regle` : formulation de la règle.
- `explication` : explications associées lorsqu’elles sont disponibles.
- `exemples_incorrects` : exemples fautifs, séparés par ` | ` lorsque plusieurs exemples sont regroupés.
- `corrections` : corrections correspondantes.
- `remarques` : notes complémentaires ou limites indiquées dans la source.
- `page_section` : page(s) ou section d’origine.

## Note de fidélité

L’extraction a été réalisée par analyse du PDF. Pour certaines règles de ponctuation/typographie, le contenu récupéré indique explicitement « voir document source » au lieu de restituer les exemples détaillés; ces marqueurs ont été conservés plutôt que d’inventer des données. Les exemples sont conservés dans la langue et avec la ponctuation retournées par l’extraction, y compris les cas où l’exemple fautif/corrigé semble identique ou présente une anomalie de transcription.

## Source

PDF média fourni par l’utilisateur : `2beb0857-0808-5c1a-b44f-dbeccf3ec35d`.
