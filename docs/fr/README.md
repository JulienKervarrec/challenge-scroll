# Parcours français — challenge-scroll

Lecture guidée, en 31 chapitres, des contrats `ERC20` et `SimpleTokenSwap` et du script `index.ts` (0x Challenge on Scroll). Lecture statique du code ; aucune installation, exécution ou appel RPC n'est réalisé, et aucun audit n'est revendiqué.

## Token ERC-20 et périmètre

1. [Périmètre du parcours](01-perimetre.md)
2. [Le token ERC-20](02-token-erc20.md)
3. [Création et destruction de l'offre](03-mint-et-burn.md)
4. [Allowances et transferFrom](04-allowance.md)
5. [Transferts du token](05-transfer.md)

## Flux de swap 0x / Scroll

6. [Routeur et token WETH](06-swap-router.md)
7. [Cotation et calldata](07-quote-et-calldata.md)
8. [Signature Permit2](08-permit2.md)
9. [Transaction brute](09-transaction-raw.md)
10. [Protection contre le slippage](10-slippage.md)
11. [Deadline du swap](11-deadline.md)
12. [Niveau de frais](12-fee-tier.md)
13. [Appels externes et ordre des effets](13-appels-externes.md)
14. [Approbation du routeur](14-approvals.md)
15. [Destinataire de la sortie](15-recipient.md)
16. [Gestion des erreurs](16-erreurs.md)
17. [Observabilité de l'envoi](17-observabilite.md)
18. [Contexte de réseau](18-contexte-reseau.md)
19. [Checklist d'intégration](19-checklist-integration.md)
20. [Limites et suite de revue](20-limites.md)

## Invariants, robustesse et reproductibilité

21. [Invariants ERC-20 à préserver](21-invariants-erc20.md)
22. [Compatibilité avec les tokens](22-compatibilite-tokens.md)
23. [Réduction des allowances](23-approval-zero.md)
24. [Reçu et finalité](24-recepisse-onchain.md)
25. [Atomicité du swap](25-atomicite-swap.md)
26. [Pool et liquidité disponible](26-pool-et-liquidite.md)
27. [Limite de prix sqrtPriceLimitX96](27-sqrt-price-limit.md)
28. [Destinataire et rejeu applicatif](28-recipient-et-rejeu.md)
29. [Domaine EIP-712](29-domain-eip712.md)
30. [Secrets et signature locale](30-secrets-et-signature.md)
31. [Périmètre reproductible](31-perimetre-reproductible.md)

[Retour au projet](../../README.md).
