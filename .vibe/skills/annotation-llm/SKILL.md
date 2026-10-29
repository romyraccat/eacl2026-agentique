---
name: annotation-llm
description: Méthode d'annotation lemme + POS d'un échantillon TSV. À utiliser pour annoter des phrases de data/echantillon/ en zero-shot ou few-shot.
---
# Méthode
1. Lire le template de la variante demandée dans data/prompt-templates/.
2. Pour le few-shot, prendre les exemples dans le train, jamais dans le test.
3. Annoter token par token, sortie TSV : token, lemme, POS.
4. Garder exactement les tokens et leur ordre.
5. Écrire dans outputs/ et résumer.
