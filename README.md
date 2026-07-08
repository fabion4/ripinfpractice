# Suite RIPAM · INF — Funzionario Informatico

Applicazione di studio completa per la **prova scritta tecnica** del concorso RIPAM/Formez PA, profilo **Funzionario Informatico** (codici INF). Un unico file HTML, senza dipendenze e senza server: si apre nel browser, funziona anche offline e salva i progressi in locale.

**Demo:** apri `index.html` nel browser, oppure vai su https://fabion4.github.io/ripinfpractice.

## Perché questa app

La prova scritta RIPAM è un test di **40 quesiti in 60 minuti** (25 di materia, 8 di logica, 7 situazionali) con punteggio **+0,75** per risposta esatta, **−0,25** per errata, **0** per omessa e soglia di idoneità **21/30**. La banca dati ufficiale non viene pubblicata prima della prova: l'unica preparazione efficace è allenarsi con quesiti realistici e un metodo solido.

Il metodo dell'app applica le tecniche con la migliore evidenza scientifica nella letteratura sull'apprendimento (practice testing e distributed practice, cfr. Donoghue & Hattie 2021; McDaniel et al. 2011; Price et al. 2024; Xu et al. 2024):

- **Recupero attivo**: quiz con feedback immediato e spiegazione dopo ogni risposta
- **Ripetizione spaziata**: flashcard con sistema Leitner a 5 livelli (intervalli 0 → 1 → 2 → 4 → 7 giorni)
- **Error quiz**: ogni quesito sbagliato entra in un registro dedicato e ne esce solo dopo 2 risposte corrette consecutive
- **Mock cronometrati**: simulazioni fedeli al formato reale, con correzione approfondita e re-test degli errori

## Funzionalità

| Sezione | Contenuto |
|---|---|
| **Piano 7 giorni** | Programma da 18 ore (2 h/giorno, 5 h nei giorni 3 e 4) con checklist e minutaggio per attività |
| **Quiz** | 124 quesiti a risposta multipla in stile RIPAM su 13 materie, con spiegazione immediata |
| **Simulazione** | 40 quesiti / 60 minuti con timer, composizione reale (25+8+7), punteggio ufficiale, navigazione libera, revisione finale quesito per quesito |
| **Flashcard** | 58 carte cloze atomiche (norme, articoli, sigle, definizioni) con ripetizione spaziata |
| **Errori** | Registro automatico degli errori con re-test mirato |
| **Statistiche** | Percentuale di correttezza per materia, storico dei mock, backup/ripristino |

### Materie coperte

Pesate secondo le proporzioni stimate del bando (~60-65% tecnica, ~25-30% giuridica):

- Reti e protocolli · Sicurezza informatica e GDPR · Basi di dati e SQL · Ingegneria del software · Project e service management (ITIL, PRINCE2, Scrum) · Sistemi operativi e cloud
- CAD e digitalizzazione della PA (SPID, PEC, PDND, PagoPA, ANPR, Piano Triennale AgID, PSN/ACN, NIS 2)
- Diritto amministrativo (L. 241/1990, FOIA, anticorruzione) · Diritto penale e Costituzione · Pubblico impiego (D.Lgs. 165/2001, DPR 62/2013)
- Inglese B1 · Logica · Quesiti situazionali (con punteggio reale 0,75 / 0,375 / 0)

## Utilizzo

1. Apri `index.html` in un browser moderno (Chrome, Edge, Firefox, Safari)
2. Giorno 1: parti dalla **simulazione diagnostica** per la baseline
3. Segui il piano giornaliero; leggi sempre le spiegazioni degli errori
4. Chiudi ogni giornata con il **quiz errori** e le **flashcard in scadenza**
5. Obiettivo prima dell'esame: media mock ≥ 24/30 e nessuna materia sotto il 60%

### Strategia d'esame integrata

- Rispondi solo se elimini almeno un'opzione (la penalità −0,25 punisce il caso puro)
- Sui situazionali rispondi **sempre**: non c'è mai penalità e la risposta neutra vale +0,375
- Ritmo: circa 1 minuto e 30 secondi a quesito

## Salvataggio dei dati

I progressi (piano, errori, flashcard, storico mock) sono salvati automaticamente nel **localStorage** del browser: sopravvivono alla chiusura e al riavvio, ma sono legati a browser + dispositivo e vengono persi in navigazione privata o cancellando i dati di navigazione.

Per sicurezza usa **Statistiche → Esporta progressi (.json)** a fine giornata e **Importa backup** per ripristinare (anche su un altro dispositivo o sulla versione online).

## Deploy su GitHub Pages

1. Repository pubblico con `index.html` nella root
2. **Settings → Pages → Branch: main → Save**
3. Dopo 1-2 minuti l'app è su `https://<username>.github.io/<repo>/`

## Tecnologie

HTML + CSS + JavaScript vanilla in un singolo file (~95 KB). Nessuna dipendenza, nessuna build, nessun backend. Font: Titillium Web (il carattere ufficiale della PA italiana), con fallback di sistema se offline.

## Avvertenze

- I quesiti sono materiale di **esercitazione** redatto sulla base delle materie del bando e delle banche dati di concorsi analoghi: non provengono dalla banca dati ufficiale, che non è pubblica.
- La ripartizione dei 25 quesiti di materia per argomento è una **stima**: il bando non pubblica pesi per sotto-materia. Ricalibra lo studio sulle tue statistiche.
- Verifica sempre formato, date e materie sul **bando ufficiale** e sul portale inPA: fanno fede solo le fonti ufficiali.
- Normativa aggiornata a inizio 2026 (incl. abrogazione dell'abuso d'ufficio ex L. 114/2024, D.Lgs. 138/2024 di recepimento NIS 2, D.Lgs. 36/2023).

## Licenza

Uso personale per la preparazione al concorso. Il contenuto dei quesiti è originale; i riferimenti normativi citati appartengono alle rispettive fonti ufficiali.

---

*In bocca al lupo per la prova!*
