# Allowances et transferFrom

Le flux de swap dépend d’une allowance : SimpleTokenSwap appelle transferFrom pour déplacer le token vendu. L’autorisation est ensuite gérée séparément par approve vers le routeur. Les intégrateurs doivent vérifier le token, le spender, le montant et la durée de vie de chaque allowance. Une allowance résiduelle ou illimitée augmente l’impact d’une erreur d’adresse ou de clé.
