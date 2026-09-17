# Checklist d’intégration

Avant un swap, vérifier tokenIn, tokenOut, amountIn, amountOutMinimum et recipient. Vérifier ensuite les adresses du routeur, la chaîne, le niveau de frais et l’éventuelle donnée Permit2. Après envoi, conserver le hash et relire le reçu sur l’explorateur approprié. Cette checklist est directement dérivée des paramètres de SimpleTokenSwap.swap et du parcours index.ts.
