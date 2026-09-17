# Domaine EIP-712

Lorsque quote.permit2.eip712 est fourni, index.ts s’appuie sur les données typées retournées par la cotation. Le domaine EIP-712 lie normalement une signature à un protocole, une chaîne et un contrat selon les champs présentés. Le script ne doit pas reconstruire silencieusement ces champs à partir d’une autre source. Avant signature, l’interface doit afficher un résumé compréhensible et vérifier la cohérence du domaine.
