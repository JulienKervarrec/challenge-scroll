# Destinataire et rejeu applicatif

La fonction swap ne contient pas de nonce métier ni d’identifiant de commande visible. La protection contre les exécutions répétées dépend donc du contexte de transaction et des paramètres fournis. index.ts prépare chaque envoi à partir d’une cotation et d’une signature éventuelle. Une application doit empêcher qu’une même intention utilisateur soit soumise plusieurs fois par erreur.
