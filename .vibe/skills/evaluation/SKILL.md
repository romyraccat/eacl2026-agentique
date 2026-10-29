---
name: evaluation
description: Calcul d'exactitude lemme et POS contre un gold TSV. À utiliser pour évaluer une sortie d'annotation.
---
# Méthode
1. Vérifier que sortie et gold ont le même nombre de tokens.
2. Lancer uv run python scripts/evaluer.py <sortie> <gold>.
3. Rendre exactitude lemme, exactitude POS, 5 erreurs typiques.
Cas de test : un fichier identique au gold donne 100 %.
