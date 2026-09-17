# Le token ERC-20

TONCONTRAT hérite d’ERC20 et configure son nom et son symbole dans le constructeur. L’offre initiale est frappée vers l’adresse qui déploie le contrat au moyen de _mint. Les fonctions standard comme balanceOf, transfer et approve restent fournies par la bibliothèque héritée. Une revue doit donc distinguer le comportement local du contrat et les garanties de l’implémentation ERC-20 utilisée.
