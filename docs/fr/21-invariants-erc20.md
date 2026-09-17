# Invariants ERC-20 à préserver

L’interface IERC20 impose une cohérence entre totalSupply, balanceOf, Transfer et Approval. Dans TONCONTRAT, _mint augmente l’offre et crédite le déployeur au moment de la construction. mint et burn modifient ensuite l’état monétaire ; leur visibilité publique doit être intégrée à toute analyse d’invariants. Les documents de ce parcours décrivent les chemins du code, sans affirmer une garantie économique non vérifiée.
