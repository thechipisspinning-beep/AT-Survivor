# AT in mutande

Roguelike "survivor" in un unico file HTML (`index.html`): modalità Classica, Ondate e Tower Defense.
Si gioca aprendo `index.html` nel browser; funziona anche offline (il font è incluso nel file).

## Pronto per l'app (Capacitor)
Il gioco riconosce da solo se gira dentro un'app Capacitor e usa questi plugin, se installati:

| Plugin | A cosa serve |
|---|---|
| `@capacitor/preferences` | copia nativa del salvataggio (il sistema non la cancella come la memoria del browser) |
| `@capacitor/app` | pausa automatica quando l'app va in background |
| `@capacitor-community/admob` | consenso GDPR + video con premio per rinascere |

Senza plugin (sul web) il gioco funziona lo stesso: salvataggio nel browser e rinascita gratuita.

**Prima di pubblicare con le pubblicità:** in `index.html`, blocco `ADS_CFG`, sostituire gli ID di prova
di Google con quelli del proprio account AdMob e mettere `testing:false`.

## Privacy
`PRIVACY.md` contiene l'informativa da pubblicare online (gli store chiedono un link). Compilare nome e contatto.
