# Code promo Marionnaud, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Marionnaud** depuis [shopilo.fr](https://shopilo.fr/reductions/marionnaud.fr). Renvoie les **coupons Marionnaud** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-marionnaud](https://shopilo-fr.github.io/code-promo-marionnaud/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-marionnaud
cd code-promo-marionnaud
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Marionnaud",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% de reduction sur les parfums et soins",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/marionnaud.fr"
  }
]
```

## Coupons Marionnaud disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 15% | 15% de reduction sur les parfums et soins | [shopilo.fr](https://shopilo.fr/reductions/marionnaud.fr) |

Codes actifs : **[shopilo.fr/reductions/marionnaud.fr](https://shopilo.fr/reductions/marionnaud.fr)**

## Questions frequentes

### Comment utiliser un code promo Marionnaud ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/marionnaud.fr), ajoutez les produits a votre panier sur Marionnaud et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Marionnaud ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Marionnaud les plus recents ?
La page [shopilo.fr/reductions/marionnaud.fr](https://shopilo.fr/reductions/marionnaud.fr) est mise a jour quotidiennement avec les codes promo Marionnaud, bons de reduction Marionnaud et coupons promotionnels Marionnaud les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Marionnaud

Marionnaud est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/marionnaud.fr), retrouvez les meilleurs codes promo Marionnaud, coupons Marionnaud verifies et bons de reduction Marionnaud actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-marionnaud
```

```javascript
const { fetchCoupons } = require('code-promo-marionnaud');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
