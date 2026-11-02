# SFDN · Visore v0.6.2

**Istruzioni per la prova (novità rispetto alla v0.6.1)**

_Saccadic Fixator de Noialtri · Ottica Stefanucci, Sinalunga · 2 novembre 2026_

Valgono le istruzioni precedenti. **Tutto è sperimentale e non validato: non dà indicazioni cliniche.** Se compaiono nausea, mal di testa o visione doppia fastidiosa, ferma la prova. Questa è la **tappa 2** della v0.6.

## 1. Cosa cambia

- **Nuova voce 17: Riserve fusionali.** Misura da lontano (6 m), al centro, con un **prisma virtuale** a rampa lenta, base interna e base esterna. Le altre posizioni di sguardo e il vicino arrivano nelle tappe successive.
- **Nuovo pulsante "Prova voce"** nel menu (accanto a Prova tasti).
- **Scheda soggetto:** nuovo campo **occhio dominante motorio** (destro / sinistro / non inserito), modificabile anche sulla scheda attiva.
- **Nuove impostazioni** "Riserve fusionali" nel riquadro 3.
- Tutto il resto (test 9, sfere, soglia, dicoptica, calibrazione, Prova tasti, vibrazione ferma) **non cambia**. La vibrazione non è disponibile nel browser del Pico: il modulo usa **solo suoni**.

## 2. Come si svolge la voce 17

1. Dal menu premi **17. Riserve fusionali**, poi **Inizia**. Il raggio sparisce e **non compare più nessuna scritta**.
2. Un **conto alla rovescia sonoro** (5 tic) e un suono di via. Poi il campo parte da solo.
3. Guarda il bersaglio (anello con un punto), al centro di una cornice e di una parete di puntini. Il prisma sale **lentamente e senza interruzioni**: tutto il campo si sposta nei due occhi.
4. Quando vedi **doppio**: premi il **grilletto**. Il prisma torna a zero e senti un suono.
5. Quando rivedi **una cosa sola**: premi **di nuovo** il grilletto (suono diverso, due toni). Si registra il tempo di recupero.
6. Dopo una pausa a prisma zero, con un nuovo conto alla rovescia, parte la rampa successiva (l'altra base). A fine serie il **centro si ripete** con l'ordine delle basi uguale e l'assegnazione dei pallini opposta (i pallini arrivano nella tappa 3).
7. Se **non vedi doppio fino al tetto**: il risultato è **"non raggiunta"** (mai "riserva ampia").
8. **Per fermare la prova: tieni premuto il grilletto 3 secondi.** Compaiono i risultati e il raggio. La rampa che stavi premendo a lungo è segnata come non valida.
9. Se per **30 s** non premi dopo una rottura: la rampa si sospende, si registra "fusione non recuperata", pausa di 60 s a prisma zero e la stessa rampa si ripete. Dopo **2 insuccessi di fila** la posizione si chiude.

Ogni pressione conta **una volta**: per premere di nuovo bisogna prima **rilasciare** il tasto.

## 3. Cose da sapere (e che il risultato riporta)

- **I dp sono nominali:** angolo totale = atan(dp/100), diviso a metà tra i due occhi. Vanno **confrontati con le misure fatte con la barra di prismi** sullo stesso soggetto.
- **Il ritardo di risposta gonfia il valore** (a 3 dp/s mezzo secondo di ritardo vale circa 1,5 dp): **i confronti vanno fatti alla stessa velocità** (0,5 / 1 / 2 / 3 dp/s, predefinita 1; fissa per tutta la serie e scritta nel risultato).
- **La pressione del grilletto non distingue fusione da soppressione:** se un occhio sopprime, la rottura può non comparire o comparire tardi. Il controllo dei pallini arriva nella tappa 3.
- Il visore **non ha eye tracking**: non si sa dove guarda davvero il soggetto.
- **Base interna:** immagini spostate verso l'esterno (OD a destra, OS a sinistra). **Base esterna:** al contrario.
- I **tetti** (lontano: interna 20 dp, esterna 35 dp; vicino 35 e 35, usato dalla tappa 4) e **tutti i tempi** si cambiano nelle impostazioni e si scrivono nel risultato, insieme agli interruttori (cornice, piano, grandezza) e alla scelta del pallino sopra.
- Tre **interruttori** (predefiniti accesi): cornice, piano a punti, grandezza realistica del bersaglio. Cornice a 9 gradi dal punto di fissazione (regolabile).

## 4. Prova voce

1. Dal menu premi **Prova voce**.
2. Il riquadro dice se il browser ha la **sintesi vocale**, quante voci trova e quali sono **italiane**.
3. Premi **Ascolta una frase**: dovresti **sentire una voce** che dice "Quali pallini vedi? Sopra, sotto, entrambi, nessuno".
4. **Torna al menu**: il risultato si salva e va nella mail.

Non c'è ancora nessuna logica vocale: serve solo a sapere se la voce italiana esiste. Se non c'è, preparo l'elenco delle frasi da registrare.

## 5. Cosa non è stato provato nel Pico vero

- **Tutto il modulo riserve** (nel simulatore funziona: spostamento misurato in pixel a 5, 20 e 35 dp, nessun bordo vuoto fino al tetto anche a 3 dp/s, tasti, tempi e sospensioni).
- Se la **cornice, la parete a punti e il bersaglio si leggono bene** a 6 m nel visore (circa 20 pixel per grado: il bersaglio realistico da 6 cm misura 0,57 gradi, circa 11 pixel).
- Se il **prisma, a livelli alti, dà fastidio** o fa sparire parti del campo ai bordi delle lenti.
- Se i **suoni** (conto alla rovescia, rottura, recupero, via, stop) si sentono bene e si distinguono.
- Se la pausa di 10 s, il conto da 5 s e i tempi di sospensione sono comodi.
- La **Prova voce** (esiste una voce italiana?).
- Il campo "occhio dominante motorio" e le nuove impostazioni su https.

## 6. Cosa mandarmi

| Domanda | Risposta |
|---|---|
| Voce 17: si vede lo spostamento? A che punto compare il doppio (dp)? | |
| La cornice, i puntini e il bersaglio si vedono bene? Qualche bordo vuoto o parte che sparisce a prisma alto? | |
| I suoni si sentono e si distinguono (via, rottura, recupero, conto alla rovescia)? | |
| Pausa e conto alla rovescia: troppo lunghi, troppo corti? | |
| Lo stop con il grilletto tenuto 3 s funziona? | |
| Confronto con la barra di prismi sullo stesso soggetto (base interna ed esterna, da lontano) | |
| Prova voce: cosa scrive il riquadro? Si sente la voce? | |
| Fastidi, durata, stanchezza | |
| Dalla Prova tasti (v0.5D o v0.6.1): quali **assi** (numero) si muovono con la leva e con quale segno su / giù / destra / sinistra | |

Dalla pagina: **Invia i risultati per email** (la voce 17 e la Prova voce sono incluse).
