# Périmètre du parcours

Ce dépôt regroupe un exemple de token ERC-20 et un flux de swap destiné à Scroll. Le contrat TONCONTRAT s’appuie sur l’implémentation ERC-20 héritée, tandis que SimpleTokenSwap délègue l’échange à un routeur compatible Uniswap. Le script index.ts prépare une cotation, une éventuelle signature Permit2, puis une transaction brute. Ce chapitre fixe le périmètre de la lecture statique ; aucune installation ni exécution n’est réalisée.
