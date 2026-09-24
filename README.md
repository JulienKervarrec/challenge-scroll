# challenge-scroll

Solution du **0x Challenge on Scroll** (échange WETH → wstETH via l'API 0x Swap et Permit2), accompagnée d'un parcours de lecture en français des contrats et du script.

Le script `index.ts` :

1. liste les sources de liquidité disponibles sur Scroll ;
2. récupère un prix puis une cotation 0x avec frais d'affiliation et collecte du surplus ;
3. affiche la répartition des sources de liquidité et les taxes d'achat/vente ;
4. signe le message Permit2 renvoyé par la cotation, l'ajoute au calldata, puis signe et envoie la transaction.

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.ts` | Script principal : cotation 0x, Permit2, envoi de la transaction sur Scroll. |
| `abi/weth-abi.ts` | ABI du contrat WETH9 utilisé par `index.ts`. |
| `ERC20` | Contrat ERC-20 aplati (hérité d'OpenZeppelin). |
| `SimpleTokenSwap` | Contrat de swap aplati délégant à un routeur compatible Uniswap V3. |
| `docs/fr/` | Parcours de lecture en 31 chapitres. Voir le [sommaire](docs/fr/README.md). |

## Utilisation

```bash
npm install
cp .env.example .env   # renseigner les variables ci-dessous
npx tsx index.ts
```

Variables d'environnement attendues par `index.ts` :

| Variable | Description |
| --- | --- |
| `PRIVATE_KEY` | Clé privée du compte (sans le préfixe `0x`). |
| `ZERO_EX_API_KEY` | Clé d'API 0x. |
| `ALCHEMY_HTTP_TRANSPORT_URL` | URL RPC HTTP pour Scroll. |

> Ne jamais committer de clé privée ni de fichier `.env`. Utiliser un compte de test.

## Parcours de lecture

Les 31 chapitres de [`docs/fr`](docs/fr/README.md) décrivent les symboles observés dans `ERC20`, `SimpleTokenSwap` et `index.ts` : token ERC-20, flux de swap, Permit2, slippage, invariants et limites. Lecture statique du code, sans exécution ni audit revendiqué.

## Licence

Le code hérité (OpenZeppelin, interfaces Uniswap) conserve sa licence MIT d'origine, indiquée en tête des fichiers concernés.
