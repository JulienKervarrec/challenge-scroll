# Limite de prix sqrtPriceLimitX96

SimpleTokenSwap fixe sqrtPriceLimitX96 à zéro dans ExactInputSingleParams. Cette valeur indique l’absence de limite de prix explicite dans ce chemin. La protection économique restante repose alors principalement sur amountOutMinimum. Les interfaces doivent rendre cette absence visible lorsqu’elles présentent les paramètres de risque à l’utilisateur.
