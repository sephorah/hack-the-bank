# Raccourcis et commandes de la démo Solen

## Dans l'app : une seule touche, sans Alt ni Maj

Attendre que la page soit chargée : une touche pressée avant ne fait rien.

| Touche | Effet |
|---|---|
| `S` | Retire ou remet **S**olen (démo avant / après). Le choix est gardé si on recharge la page. |
| `R` | **R**emet le score de vigilance et les badges à zéro. À faire avant chaque démo. |
| `F` | Ouvre la page **F**ournisseurs dans un nouvel onglet. |
| `P` | É**p**ingle ou désépingle le panneau Solen. Il est désépinglé au chargement : Solen n'analyse aucun mail, aucun appel à Mistral. |
| `1` | Nuvio Cloud (hébergeur) : faux RIB |
| `2` | Support informatique : faux renouvellement de double authentification (`arkos-systerns.fr`) |
| `3` | Jean-Pierre Durand : faux président |
| `4` | Marc Lefèvre, le DAF : mail urgent légitime, aucune alerte |
| `5` | Banque Horizon : faux conseiller bancaire (bonus) |
| `6` | Delivery Partners : facture de conseil depuis `de1ivery-partners.fr` (bonus) |

## Lancer l'app (dans le dossier `garde-fou/`)

| Commande | Effet |
|---|---|
| `npm run dev` | Lance l'app sur http://localhost:3000, avec le vrai Mistral (clé dans `.env.local`). |
| `npm run build && npm start` | Version plus rapide, conseillée pour le jour J. |
| `SOLEN_AI=secours npm run dev` | N'appelle jamais Mistral : réponses écrites à l'avance, coût nul. |
| `npm test` | Lance les 60 tests, dont les 26 attaques. |

## Avant de passer devant le jury

1. Lancer l'app, appuyer sur `P` (ouvre le panneau), puis sur `1` à `6` : chaque analyse est gardée en mémoire, la démo devient instantanée.
2. `R` pour remettre le score à zéro.
3. `1`, puis `S` pour retirer Solen, afin de commencer par l'écran « sans Solen ».
4. Si Mistral ne répond pas, Solen bascule seul sur les réponses de secours. La vidéo reste le dernier recours.
