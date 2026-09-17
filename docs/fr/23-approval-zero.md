# Réduction des allowances

Le swap approuve le routeur pour amountIn après avoir transféré les tokens au contrat. La séquence ne documente pas de remise à zéro préalable. Avec un token qui impose cette étape, approve peut se comporter différemment de l’attendu. La politique d’intégration doit définir une allowance minimale, sa révocation et la manière de traiter un échec d’approbation.
