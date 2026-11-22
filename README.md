# Andrea in mutande

Roguelike "survivor" in un unico file HTML (`index.html`). Si gioca aprendo `index.html` nel browser
e funziona anche offline (il font è incluso nel file). Testi in italiano e in inglese (Menu → Opzioni → Lingua).

## Contenuti
- **Modalità:** Classica (vittoria a 30 minuti, poi infinita), Ondate (mercatino ogni 3 ondate),
  Tower Defense (3 percorsi, il personaggio aiuta le torri, velocità x2, bersagli e specializzazioni).
- **5 personaggi:** Andrea, Kevin, Christian, Thomas, Nonno, ognuno con arma iniziale e statistiche proprie.
- **14 armi** con due evoluzioni, **8 oggetti passivi**, **8 Fusioni** (arma Lv.5 + passivo).
- **Level-up** con Rilancia, Escludi e Salta.
- **6 animali compagni** (topo, gatto, pipistrello, ragno, rana, gufo) da adottare e allenare.
- **Nemici:** 3 nuovi tipi (lumaca che sputa, fungo che esplode, melma che si divide), élite con forziere, 5 boss.
- **3 mappe:** Cantina, Giardino di notte, Cucina.
- **Negozio** con 10 potenziamenti permanenti, **19 missioni** con premi e sblocchi.
- Tutorial alla prima partita, menu Opzioni (volumi, vibrazione, qualità grafica, lingua).

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
