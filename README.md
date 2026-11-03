# SFDN Visore

Programma sperimentale di prova per il visore Pico Neo 3 Pro (Saccadic Fixator de Noialtri, Ottica Stefanucci, Sinalunga). Versione v0.6.2 (tappa 2 della v0.6: Riserve fusionali, motore del prisma da lontano al centro; Prova voce).

**Tutto è sperimentale e non dà indicazioni cliniche.**

- Programma: `index.html` (un solo file, funziona offline, nessuna libreria esterna).
- Versioni precedenti (stesso indirizzo, stessi dati del browser): `versioni/SFDN_Visore_v0.6.1.html` (vibrazione e clic joystick nella Prova tasti, email nelle impostazioni), `versioni/SFDN_Visore_v0.5D.html` (Prova tasti, pulsanti prove/azzera), `versioni/SFDN_Visore_v0.5ABC.html` (con i reticoli, archiviati nella v0.5D), `versioni/SFDN_Visore_v0.5B2.html` e `versioni/SFDN_Visore_v0.5AB.html`.
- Istruzioni per la prova: `istruzioni/ISTRUZIONI_VISORE_v0.6.2.md` (novità rispetto alla v0.6.1), `istruzioni/ISTRUZIONI_VISORE_v0.6.1.md` (novità rispetto alla v0.5D), `istruzioni/ISTRUZIONI_VISORE_v0.5D.md` (novità rispetto alla v0.5ABC) e `istruzioni/ISTRUZIONI_VISORE_v0.5ABC.md`.
- I dati dei soggetti restano nel browser del dispositivo e non sono mai caricati qui.

## Giochi SFDN "Ape rossa" e "Ape e palloncino" (v0.2)

Giochi sperimentali di allenamento visivo, **separati dal Visore** (altro file, altri dati). **Non sono un trattamento validato**: sessioni brevi e con supervisione.

- Programma: `gioco/index.html` (un solo file, funziona offline; le voci sono opzionali). Indirizzo: `https://daziele74.github.io/sfdn-visore/gioco/`. È un menu con due giochi: **1 APE ROSSA** (nuovo: palloncini blu a caduta o fermi, ape che si avvicina e al limite vicino diventa rossa e pulsante; due mani; velocità adattiva) e **2 APE E PALLONCINO** (la v0.1, invariata).
- Voci registrate: `audio/01.wav` ... `audio/07.wav` (gioco 2). Le voci 08-12 del gioco 1 non sono ancora registrate: se mancano il gioco usa solo i toni.
- Istruzioni brevi: `gioco/ISTRUZIONI_GIOCO_v0.2.md` (la v0.1 resta in `gioco/ISTRUZIONI_GIOCO_v0.1.md`).
- I dati dei giochi restano nel browser del dispositivo, in una chiave separata da quella del Visore (ogni partita porta l'id del gioco); dal Visore si leggono soltanto (nome e soglia stereo).
