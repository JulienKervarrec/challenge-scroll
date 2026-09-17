# Routeur et token WETH

Le constructeur de SimpleTokenSwap reçoit _swapRouter et _WETH, puis stocke ces adresses. Le swap utilise l’interface ISwapRouter et appelle exactInputSingle. La variable WETH est exposée publiquement mais n’est pas utilisée dans la fonction swap visible ici. Une intégration doit donc vérifier que les adresses configurées correspondent bien au réseau et au routeur attendu.
