# CosmoLive — Il Sistema Solare in diretta

App web in un solo file (`index.html`), senza installazioni.

## Apri l'app

**👉 https://draxarden.github.io/cosmo-live/**

Funziona da computer, tablet e telefono, con tutte le dirette.

### Aggiornare il sito

Ogni modifica a `index.html` caricata su questo repository (ramo `main`) viene pubblicata in automatico in circa un minuto.

### Usarla senza internet… quasi

Puoi anche scaricare `index.html` e aprirlo con un doppio clic: funziona tutto tranne la diretta YouTube, che YouTube blocca nei file aperti dal computer.

## Collegamenti diretti

- `draxarden.github.io/cosmo-live/#saturn` apre direttamente su Saturno (vale per ogni corpo: `#mars`, `#europa`, `#titan`…)
- `draxarden.github.io/cosmo-live/#live` apre direttamente la sezione Live

## Fonti dati (tutte gratuite, senza registrazione)

| Contenuto | Fonte |
|---|---|
| Notizie | Spaceflight News API (articoli in inglese) |
| Foto e video | NASA Image and Video Library |
| Posizione ISS | wheretheiss.at |
| Il Sole | NASA SDO, ESA/NASA SOHO |
| La Terra | NOAA GOES-19 / GOES-18, NASA DSCOVR EPIC |
| Dirette video | YouTube: NASA, Sen (ISS) · Asahi Astro LIVE (Subaru, CFHT, ALMA, Kiso) · explore.org e Starlapland (aurore) · NASASpaceflight (Starbase, Space Coast) |

## Note

- Le posizioni dei pianeti sono calcolate per la data reale (orbite circolari approssimate). Le distanze sono in scala logaritmica, così ci stanno tutti. Le lune più veloci sono rallentate per renderle leggibili.

## Aggiungere o cambiare una diretta

Le dirette sono nell'elenco `STREAM_GROUPS` dentro `index.html`. Ognuna ha un nome, il canale, l'`id` del video YouTube (la parte dopo `watch?v=`) e il fuso orario del luogo. Se una diretta finisce, l'app passa da sola alla successiva della stessa categoria. Per sostituirla basta cambiare l'`id`.
