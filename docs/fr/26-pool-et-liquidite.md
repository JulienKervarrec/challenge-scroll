# Pool et liquidité disponible

exactInputSingle reçoit tokenIn, tokenOut et un fee de 3000, ce qui détermine le pool Uniswap V3 recherché. La présence d’une interface de routeur ne garantit pas qu’un pool liquide existe pour cette combinaison. La cotation de index.ts doit être contrôlée contre le même réseau et les mêmes paramètres. Une revue utile consigne aussi l’impact d’une liquidité insuffisante sur amountOut.
