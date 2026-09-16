# Tableau des types de fautes — hiérarchie du PDF

Le PDF source est hiérarchique : catégorie → groupe → sous-code → règle → exemples X/v.

Catégories : G (Orthographe grammaticale), P (Ponctuation et typographie), S (Syntaxe), U (Orthographe d’usage), V (Vocabulaire).

Le code atomique doit être le sous-code lorsqu’il existe, par exemple `G1.1`, et non simplement `G1`. Le groupe parent doit être conservé séparément (`G1`), tout comme la catégorie (`G`).

Le rapport `sous_regles_extraction_rapport.md` recense les sous-codes et le comptage : G 23, P 65, S 43, U 3, V 7, soit 141 sous-règles recensées.

Le CSV principal doit utiliser : `categorie_id`, `categorie`, `groupe`, `code`, `regle`, `explication`, `exemples_incorrects`, `exemples_corrects`, `source_pages`.

Source : PDF média `2beb0857-0808-5c1a-b44f-dbeccf3ec35d`.
