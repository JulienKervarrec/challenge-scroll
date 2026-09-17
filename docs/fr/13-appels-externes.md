# Appels externes et ordre des effets

La fonction swap appelle successivement transferFrom, approve et swapRouter.exactInputSingle. Ces appels externes constituent les points à examiner lors d’une revue de sécurité. Le code vérifie les retours booléens des deux appels ERC-20, puis contrôle amountOut. Ce chapitre signale une surface d’analyse ; il ne conclut pas à une réentrance exploitable sans preuve supplémentaire.
