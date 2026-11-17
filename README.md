# CosmoLive — Il Sistema Solare in diretta

App web in un solo file (`index.html`), senza installazioni.

## Come aprirla

**Modo rapido:** doppio clic su `index.html`. Funzionano mappa, notizie, foto, video NASA, posizione della ISS e immagini live di Sole e Terra.

**Modo completo (consigliato):** serve anche per vedere la diretta YouTube NASA dentro l'app (YouTube blocca i video aperti come file locale).
Apri un terminale nella cartella dell'app e scrivi:

```
python3 -m http.server 8000
```

(su Windows: `python -m http.server 8000`), poi vai su <http://localhost:8000> nel browser.

## Collegamenti diretti

- `index.html#saturn` apre direttamente su Saturno (vale per ogni corpo: `#mars`, `#europa`, `#titan`…)
- `index.html#live` apre direttamente la sezione Live

## Fonti dati (tutte gratuite, senza registrazione)

| Contenuto | Fonte |
|---|---|
| Notizie | Spaceflight News API (articoli in inglese) |
| Foto e video | NASA Image and Video Library |
| Posizione ISS | wheretheiss.at |
| Il Sole | NASA SDO, ESA/NASA SOHO |
| La Terra | NOAA GOES-19 / GOES-18, NASA DSCOVR EPIC |
| Diretta video | canale YouTube NASA |

## Note

- Le posizioni dei pianeti sono calcolate per la data reale (orbite circolari approssimate). Le distanze sono in scala logaritmica, così ci stanno tutti. Le lune più veloci sono rallentate per renderle leggibili.
- Per pubblicarla online basta caricare `index.html` su un hosting statico qualsiasi (GitHub Pages, Netlify, Vercel).
