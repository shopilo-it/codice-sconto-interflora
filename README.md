# Codice sconto Interflora, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Interflora** da [shopilo.it](https://shopilo.it/negozi/interflora.it). Restituisce **coupon Interflora** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-interflora](https://shopilo-it.github.io/codice-sconto-interflora/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-interflora
cd codice-sconto-interflora
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Interflora",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su consegna fiori a domicilio",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/interflora.it"
  }
]
```

## Coupon Interflora disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su consegna fiori a domicilio | [shopilo.it](https://shopilo.it/negozi/interflora.it) |

Codici attivi: **[shopilo.it/negozi/interflora.it](https://shopilo.it/negozi/interflora.it)**

## Domande frequenti

### Come utilizzo un codice sconto Interflora?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/interflora.it), aggiungi i prodotti al carrello su Interflora e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Interflora?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Interflora piu recenti?
La pagina [shopilo.it/negozi/interflora.it](https://shopilo.it/negozi/interflora.it) viene aggiornata quotidianamente con i codici sconto Interflora, voucher Interflora e coupon promozionali Interflora piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Interflora

Interflora e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/interflora.it) trovi i migliori codici sconto Interflora, coupon Interflora verificati e voucher Interflora attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-interflora
```

```javascript
const { fetchCoupons } = require('codice-sconto-interflora');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
