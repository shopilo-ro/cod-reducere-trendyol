# Cod reducere Trendyol — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Trendyol** de pe [shopilo.ro](https://shopilo.ro/magazin/trendyol.com). Returneaza **cupoane Trendyol** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-trendyol](https://shopilo-ro.github.io/cod-reducere-trendyol/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-trendyol
cd cod-reducere-trendyol
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Trendyol",
    "code": "SHOPILO30",
    "discount": "30%",
    "description": "30% reducere la comenzile din aplicatie",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/trendyol.com"
  }
]
```

## Cupoane Trendyol disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 30% | 30% reducere la comenzile din aplicatie | [shopilo.ro](https://shopilo.ro/magazin/trendyol.com) |

Codurile active: **[shopilo.ro/magazin/trendyol.com](https://shopilo.ro/magazin/trendyol.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Trendyol?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/trendyol.com), adauga produsele in cos pe Trendyol, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Trendyol?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Trendyol?
Pagina [shopilo.ro/magazin/trendyol.com](https://shopilo.ro/magazin/trendyol.com) este actualizata zilnic cu cele mai noi cod reducere Trendyol, voucher Trendyol si cupon promotional Trendyol.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Trendyol

Trendyol este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/trendyol.com) cele mai bune cod reducere Trendyol, cupoane Trendyol verificate si voucher Trendyol active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-trendyol
```

```javascript
const { fetchCoupons } = require('cod-reducere-trendyol');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
