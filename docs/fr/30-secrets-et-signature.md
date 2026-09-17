# Secrets et signature locale

index.ts utilise un compte configuré pour signer une transaction brute. La clé privée ne doit jamais être exposée dans le dépôt, les journaux ou une URL. Le fait que le script signe localement ne précise pas à lui seul le dispositif de garde utilisé. Une procédure de production doit isoler les secrets, limiter les permissions et demander une validation explicite des paramètres critiques.
