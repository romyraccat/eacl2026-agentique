# eacl2026-agentique

Lemmatisation et POS-tagging de langues historiques (grc, hye, kat, syc)
par annotateurs LLM, en zero-shot et few-shot (5, 50, 500 exemples).

## Python
- uv add, uv run python, uv run pytest.
- Jamais pip, jamais python seul.
- Ne jamais modifier uv.lock ni .venv/.

## Règles
- Répondre en français.
- Ne jamais écrire de clé API dans un fichier ni l'afficher.
- results/ et pie-baseline/ : lecture seule (résultats du papier).
- Les fichiers de test (data/corpus/*test*) sont le gold : seuls
  l'évaluateur et les scripts d'évaluation les lisent.
- Petits volumes (échantillon) : traitement direct par un sous-agent.
  Gros volumes : écrire et tester un script, ne pas annoter token par token.
- Sorties volumineuses : dans outputs/, pas dans la conversation.

## Délégation
- annotateur : annoter data/echantillon/.
- evaluateur : calculer les scores lemme / POS.
- relecteur : relire templates et tagsets.
