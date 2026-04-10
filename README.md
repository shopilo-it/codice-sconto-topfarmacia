# Codice sconto TopFarmacia, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto TopFarmacia** da [shopilo.it](https://shopilo.it/negozi/topfarmacia.it). Restituisce **coupon TopFarmacia** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-topfarmacia](https://shopilo-it.github.io/codice-sconto-topfarmacia/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-topfarmacia
cd codice-sconto-topfarmacia
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "TopFarmacia",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su farmaci e integratori online",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/topfarmacia.it"
  }
]
```

## Coupon TopFarmacia disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su farmaci e integratori online | [shopilo.it](https://shopilo.it/negozi/topfarmacia.it) |

Codici attivi: **[shopilo.it/negozi/topfarmacia.it](https://shopilo.it/negozi/topfarmacia.it)**

## Domande frequenti

### Come utilizzo un codice sconto TopFarmacia?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/topfarmacia.it), aggiungi i prodotti al carrello su TopFarmacia e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon TopFarmacia?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher TopFarmacia piu recenti?
La pagina [shopilo.it/negozi/topfarmacia.it](https://shopilo.it/negozi/topfarmacia.it) viene aggiornata quotidianamente con i codici sconto TopFarmacia, voucher TopFarmacia e coupon promozionali TopFarmacia piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su TopFarmacia

TopFarmacia e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/topfarmacia.it) trovi i migliori codici sconto TopFarmacia, coupon TopFarmacia verificati e voucher TopFarmacia attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-topfarmacia
```

```javascript
const { fetchCoupons } = require('codice-sconto-topfarmacia');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
