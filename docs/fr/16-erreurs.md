# Gestion des erreurs

Le contrat utilise require pour vérifier les retours de transferFrom et approve, puis pour contrôler amountOut. Le script index.ts enveloppe son parcours dans une gestion d’erreur qui journalise l’échec. Ces deux niveaux ne couvrent pas les mêmes causes : un revert on-chain et une erreur de préparation locale doivent être distingués. Les messages d’erreur doivent rester associés au contexte de la transaction examinée.
