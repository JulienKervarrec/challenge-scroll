# Approbation du routeur

Après avoir reçu les tokens, SimpleTokenSwap approuve le routeur pour amountIn. L’approbation est recalculée à chaque swap au lieu d’être documentée comme une autorisation permanente. La revue doit vérifier le comportement des tokens qui exigent une remise à zéro avant de modifier une allowance non nulle. Les opérateurs doivent aussi confirmer que swapRouter reste l’adresse de confiance enregistrée au constructeur.
