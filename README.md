# Lumenar — documenti legali pubblici

Questo repository esiste per **una sola cosa**: dare all'informativa sulla privacy di
Lumenar un indirizzo web pubblico, raggiungibile senza login, da usare nella scheda
Google Play Console.

Non contiene codice dell'app. Contiene solo la pagina pubblica.

## URL pubblici

| URL | Cosa serve |
|---|---|
| https://tommasolucchesi.github.io/lumenar-legal/ | **URL canonico da mettere in Play Console** (sezione *Contenuto dell'app → Informativa sulla privacy*) |
| https://tommasolucchesi.github.io/lumenar-legal/privacy-policy.html | Reindirizza al canonico, come riserva se qualcuno usa il nome del file |

## Come si aggiorna

Copia il testo aggiornato sopra `index.html` e fai push: GitHub Pages ripubblica da sé
in circa un minuto.

```bash
cp "C:/Users/lucch/AppData/Local/hermes/lumenar-app/docs/privacy-policy.html" index.html
git add index.html && git commit -m "Aggiorna informativa" && git push
```

Il file sorgente vive in `lumenar-app/docs/privacy-policy.html`. **Questa è una copia:
se si aggiorna il sorgente e non si copia qui, la pagina pubblica resta indietro.**

## Stato

La pagina è la versione 3.0 del 20 ottobre 2026, con **segnaposto ancora aperti**:
`[INDIRIZZO]`, `[EMAIL DI CONTATTO]`, `[DA CONFERMARE]`. Va ripubblicata quando
l'indirizzo del titolare e l'email di supporto saranno reali: fino ad allora **non va
usata come URL definitivo in Play Console**.

## Dominio proprio (facoltativo)

Lo stesso sito può servire `lumenar.app` (o qualunque dominio) gratis: *Settings →
Pages → Custom domain*. In alternativa il file può essere spostato su Cloudflare Pages
o Netlify senza cambiare nulla del testo.
