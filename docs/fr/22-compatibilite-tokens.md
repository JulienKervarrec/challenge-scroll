# Compatibilité avec les tokens

SimpleTokenSwap attend que transferFrom et approve renvoient un booléen exploitable. Certains tokens historiques ont des comportements non standards, notamment des retours absents ou des frais de transfert. Le code visible utilise l’interface IERC20 et des require sur les retours. Une intégration professionnelle doit donc qualifier les tokens acceptés avant de les proposer dans l’interface.
