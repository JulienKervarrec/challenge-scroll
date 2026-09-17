# Protection contre le slippage

SimpleTokenSwap transmet amountOutMinimum à exactInputSingle et vérifie ensuite que amountOut lui est supérieur ou égal. La protection dépend donc entièrement de la valeur fournie par l’appelant ou la cotation. Une valeur nulle supprimerait la garantie économique recherchée. Les interfaces clientes doivent calculer cette borne avec une tolérance explicite et l’afficher avant signature.
