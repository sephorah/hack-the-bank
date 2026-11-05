# Démo Solen : mode d'emploi

## Avant de commencer

1. Ouvre http://localhost:3000 et attends que la page s'affiche. Le panneau Solen est fermé : rien n'est analysé, aucun crédit consommé.
2. Appuie sur `P` pour ouvrir le panneau, puis sur `1`, `2`, `3`, `4`, `5`, `6` : Solen analyse chaque mail une fois, la démo sera ensuite instantanée.
3. Appuie sur `R` (score à zéro), puis `1`, puis `S` (Solen disparaît).

**Phrase d'intro :** « Voici la boîte mail de Claire, comptable dans un éditeur de logiciels, comme beaucoup de vos entreprises. Solen est une extension installée dans son Outlook. »

## Les 4 mails de la démo

### Mail 1 : Nuvio Cloud, le faux RIB (touche `1`, puis `S`)
- **Ce que c'est :** l'hébergeur de l'entreprise annonce un changement de banque pour une facture de 18 400 €.
- **Le piège :** le mail vient vraiment de l'hébergeur, dont la boîte a été piratée. Il a l'air parfaitement normal.
- **Ce que tu fais :**
  1. Sans Solen : « Claire aurait payé. »
  2. Appuie sur `S` : le bandeau rouge et le panneau apparaissent.
  3. Montre « Nouvel IBAN » et son étiquette « Règle » : « L'expéditeur est authentique, mais l'IBAN ne l'est pas. C'est le code qui le vérifie, pas l'IA. »
  4. Clique sur « Appeler » : « Solen donne le vrai numéro, et récompense le bon réflexe. »
  5. Appuie sur `F` (nouvel onglet), montre la ligne Nuvio Cloud : « Solen connaît chaque fournisseur grâce aux 22 paiements déjà faits. Un mail ne peut jamais modifier ce profil. » Reviens sur l'onglet Outlook.

### Mail 2 : le faux support informatique (touche `2`)
- **Ce que c'est :** « votre double authentification expire, renouvelez-la avant 18 h », avec un lien.
- **Le piège :** l'adresse est `arkos-systerns.fr`, avec « rn » à la place du « m ». Le lien sert à voler les identifiants.
- **Ce que tu fais :** montre « rn » surligné en rouge : « Invisible à l'œil nu. Solen le surligne. Ici, l'IA n'est même pas appelée : le code suffit. »

### Mail 3 : Jean-Pierre Durand, le faux président (touche `3`)
- **Ce que c'est :** le « PDG » demande un virement secret de 35 000 €, depuis Gmail.
- **Le piège :** il n'y a aucun RIB à vérifier. Seule la manipulation trahit la fraude.
- **Ce que tu fais :** « C'est l'IA qui repère l'autorité, le secret et l'urgence. » Clique sur « Prévenir le DAF ».

### Mail 4 : Marc Lefèvre, le vrai DAF (touche `4`)
- **Ce que c'est :** le vrai directeur financier demande de payer une facture en urgence.
- **Le point clé :** c'est légitime, donc Solen n'alerte pas.
- **Ce que tu fais :** « Urgent, mais normal : aucune alerte. Solen ne crie pas au loup. »

**Bonus, si le jury pose une question :** `5` ouvre un faux conseiller bancaire, `6` une facture de conseil depuis `de1ivery-partners.fr` (un « 1 » à la place du « l »).

## La partie technique (4 idées)

1. **Le code vérifie, l'IA comprend.** Le code contrôle l'adresse et l'IBAN. L'IA (Mistral, européenne) repère la manipulation.
2. **L'IA ne décide jamais seule pour l'argent.** Elle ne voit pas les IBAN, et elle ne peut pas annuler une alerte. Chaque raison indique « Règle » ou « IA ».
3. **On a essayé de casser Solen :** 26 attaques, aucune ne passe aujourd'hui. Deux fois l'IA s'est fait avoir, et l'alerte a quand même sonné.
4. **Les limites :** un RIB scanné en image n'est pas vérifié, et la fraude par téléphone nous échappe.
