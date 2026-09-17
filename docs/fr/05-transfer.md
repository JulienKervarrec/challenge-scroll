# Transferts du token

Les transferts ordinaires passent par les fonctions ERC-20 héritées. Dans SimpleTokenSwap, le transfert entrant est réalisé avant l’appel au routeur, ce qui rend l’ordre des opérations important pour l’analyse du flux. Les événements et les retours attendus par ERC-20 doivent être pris en compte lors d’une intégration avec des tokens non standards. Cette lecture décrit le chemin visible dans le code sans prétendre remplacer une campagne de tests.
