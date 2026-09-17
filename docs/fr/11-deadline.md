# Deadline du swap

Le paramètre deadline de SimpleTokenSwap est fixé à block.timestamp au moment où le contrat appelle le routeur. Cela évite qu’un délai déjà expiré soit transmis dans ce chemin, mais ne fournit pas une fenêtre d’expiration choisie par l’utilisateur. Une transaction signée peut rester en attente avant son inclusion. Les interfaces devraient donc traiter séparément l’expiration côté cotation et le délai accepté par le contrat.
