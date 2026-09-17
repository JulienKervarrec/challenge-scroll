# Transaction brute

Après préparation du calldata, index.ts signe une transaction brute avec le compte configuré puis l’envoie au réseau. Le code journalise le résultat et construit une URL Scrollscan à partir du hash. Une revue opérationnelle doit vérifier la chaîne, le nonce, le gas et l’adresse du contrat avant la signature. Le fichier montre le parcours d’envoi, sans que ce parcours soit exécuté dans cette analyse.
