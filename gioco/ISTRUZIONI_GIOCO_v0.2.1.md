# SFDN Gioco v0.2.1 · Ape rossa e Ape e palloncino

**Istruzioni brevi per l'operatore**

_Ottica Stefanucci, Sinalunga · 3 novembre 2026 · versione 0.2.1_

**Sperimentale: non è un trattamento validato.** Sessioni brevi e **con supervisione**. **Interrompi subito** se compaiono disagio, mal di testa o visione doppia (tasto laterale tenuto 5 secondi, oppure B o Y tenuto 2 secondi, oppure togli il visore).

## 1. Come si apre

1. Nel browser del Pico apri `https://daziele74.github.io/sfdn-visore/gioco/`.
2. Nella pagina scrivi il nome (se in questo browser hai già usato il Visore, il nome e la soglia stereo si leggono da lì, senza modificarli).
3. Scegli le impostazioni. Per la prima prova lascia quelle predefinite: **limite vicino medio 1,5 m, 3 minuti, indizi facili, mano dominante destra, voce sì**. Accanto a **ogni casella** c'è un pulsante **i**: premilo per leggere cosa fa la casella (spiegazione semplice, con un esempio); premilo ancora per chiuderla. I testi sono anche in `SPIEGAZIONI_CASELLE.md`.
4. Premi **ENTRA IN VR**. Il primo menu in VR fa scegliere: **1 APE ROSSA** oppure **2 APE E PALLONCINO** (più PROVA AUDIO ed ESCI).

## 2. Gioco 1 · APE ROSSA

**Regola fissa: il rosso vuol dire sempre "colpisci ora".** Il rosso è riservato all'ape: nessun altro oggetto è rosso. Il segnale è rosso **più pulsazione** (l'ape si ingrandisce e rimpicciolisce e cambia tonalità), così si riconosce anche senza distinguere bene i colori.

- **Palloncini blu**, da 3 a 8 insieme (predefinito 4), a distanze diverse tra il limite vicino e circa 5 m. Si colpiscono con la **mano dominante** (predefinita destra), con il raggio e il grilletto.
- **A caduta** (predefinito): scendono in verticale a velocità costante e vanno colpiti **prima che tocchino il terreno** (il terreno si vede). **Fermi**: restano dove sono finché li colpisci. Quando un palloncino è colpito o cade a terra ne compare uno nuovo in un altro punto e a un'altra distanza.
- **L'ape** compare a caso ogni 10-20 secondi. Parte da lontano (circa 5 m) e si avvicina piano (0,5 m/s, con una variazione casuale di circa il 20%). Quando arriva al **limite vicino diventa ROSSA e pulsa** e resta così per **2,5 secondi**: in quel tempo va colpita con l'**altra mano** (la non dominante, predefinita sinistra). Poi se ne va con una breve dissolvenza.
  - Colpo **prima** del rosso: **"troppo presto"**. Nessuna penalità di punti.
  - Colpo nella finestra rossa: **giusto**; si misura il tempo di reazione dal momento in cui diventa rossa.
  - Nessun colpo: **omissione**, perdi 1 punto.
- Ogni volta l'ape cambia **direzione di partenza e di arrivo** (settori diversi da quelli degli ultimi due passaggi). Non va mai verso il viso e nessun punto del suo percorso è più vicino del limite scelto.
- **Ogni raggio colpisce solo il suo bersaglio.** Un colpo con la mano dei palloncini sull'ape, o con la mano dell'ape su un palloncino, è ignorato e registrato (nessuna penalità). I due raggi hanno colori diversi (viola per i palloncini, verde chiaro per l'ape); nessuno è rosso.
- **Punti:** palloncino colpito +1, ape colpita +5, omissione -1 (mai sotto zero).
- **Velocità adattiva** (predefinita, solo palloncini a caduta). La velocità parte sempre da V0 (predefinita 0,25 m/s). Conta **di fila**: due contatori che si azzerano a vicenda. Ogni palloncino **colpito** conta come colpito di fila e azzera le cadute di fila; ogni palloncino **a terra** conta come caduta di fila e azzera i colpiti di fila. Dopo **N colpiti di fila** (predefinito 8) la velocità **sale** di un gradino (15% di V0); dopo **M a terra di fila** (predefinito 4) **scende** di un gradino; non scende sotto il minimo (30% di V0). Dopo ogni cambio i due contatori ripartono da zero. **Una caduta isolata non fa scendere la velocità.** Si può scegliere la velocità costante.
  - **Tetto B (predefinito):** la velocità può salire **oltre V0**, fino alla velocità massima (predefinita 1,0 m/s). Se la massima è minore di V0 vale V0 (la pagina lo scrive accanto al campo). **Tetto A:** il tetto è V0 (come nella versione 0.2): la velocità può solo scendere e tornare a V0.
  - V0 e massima si possono impostare da 0,05 a 10 m/s. **Sopra circa 3 m/s quasi non si riesce a colpire:** non c'è un limite finto, serve per trovare il limite vero. Con le velocità alte la comparsa dei palloncini si accorcia in proporzione.
  - La velocità corrente è scritta in piccolo sul tabellone (per l'operatore; si può togliere dalle AVANZATE).
- **Più palloncini, più piccoli:** con 5-8 palloncini insieme il gioco calcola a inizio partita **un solo fattore di riduzione**, uguale per tutti i palloncini e fisso per tutta la partita (mai sotto la «riduzione massima», predefinita 60%), così non si toccano. I palloncini nuovi compaiono solo dove c'è posto. Se anche al minimo non ci stanno, il gioco usa un palloncino in meno e lo scrive nel riepilogo. L'area di colpo non scende mai sotto 2 gradi.
- **Compiti:** "palloncini + ape" (predefinito), "solo palloncini", "solo ape". **Una mano sola:** un solo raggio colpisce palloncini e ape. Se c'è un solo controller fa tutto lui. Per i mancini si sceglie "sinistra" come mano dominante.

## 3. Gioco 2 · APE E PALLONCINO

È il gioco della versione 0.1, **invariato**: 5 palloncini a distanze diverse; l'ape vola verso il più vicino e si posa; il giocatore lo colpisce quando l'ape è sopra. Colpo con l'ape in volo = "troppo presto"; altro palloncino = errore; se non lo colpisce entro la sosta (2 secondi) l'ape lo fa scoppiare (-1 punto). Impostazioni proprie nella pagina: facilitazione colore, sosta, volo.

## 4. Tasti (uguali nei due giochi)

| Tasto | Cosa fa |
|---|---|
| Grilletto | Colpisce, e preme i pulsanti dei menu |
| A o X (breve) | Pausa e ripresa. Nel gioco 1 il passaggio dell'ape interrotto non conta |
| B o Y tenuto 2 secondi | **Stop di emergenza**: la partita finisce e compare il riepilogo |
| **Tasto laterale (grip) tenuto 5 secondi**, di una mano o dell'altra, anche in pausa | **Interrompe** la partita, la **salva come «interrotta»** e torna al menu dei giochi con il messaggio «Partita interrotta e salvata». Mentre lo tieni premuto compare in alto un cerchio che si riempie; se lo lasci prima dei 5 secondi non succede nulla |

## 5. Impostazioni (pagina, fuori dalla VR)

- **Comuni ai due giochi:** nome, mano dominante, limite vicino (facile 2,5 m, medio 1,5 m, impegnativo 0,8 m, libero da 0,4 a 6 m), **durata a pulsanti fissi: 30 secondi, 1, 2, 3, 5, 10 minuti**, indizi (facili o difficili), voce, email dei risultati.
- **Gioco 1, BASE (si applicano subito):** compiti, palloncini (caduta o fermi), velocità adattiva sì/no, tre gruppi di suoni.
- **Gioco 1, AVANZATE (riquadro chiuso, si applicano col pulsante APPLICA):** numero di palloncini (3-8) e riduzione massima, velocità V0, tetto A o B, velocità massima, gradino, N colpiti di fila, M a terra di fila, velocità minima, velocità sul tabellone, intervallo di comparsa dell'ape, velocità e variazione dell'ape, finestra rossa, area di colpo, campo comodo, settori, una mano sola.
- **Pulsante «i»** accanto a ogni casella: cosa fa, cosa succede se la alzi o la abbassi, un esempio. **Pulsanti − e +** accanto a ogni numero (oltre alla possibilità di digitare).
- **APPLICA:** finché c'è un valore avanzato modificato e non applicato compare l'avviso giallo «Modificato, non ancora applicato», il gioco usa ancora i valori vecchi e **in VR il pulsante di avvio del gioco 1 resta spento** con la scritta «Applica prima le modifiche». APPLICA riporta nei limiti i valori fuori intervallo (e dice quali), salva e aggiorna la riga «IMPOSTAZIONI IN USO».
- **IMPOSTAZIONI IN USO:** nella pagina (riquadro del gioco 1) e in cima al menu VR del gioco 1: compiti, caduta o fermi, limite vicino, durata, palloncini, V0, tetto, massima, gradino, N e M, minimo, velocità e finestra dell'ape.
- **RIPRISTINA PREDEFINITI** (secondo clic di conferma): riporta i parametri di gioco ai valori predefiniti. **Non tocca mai** nome, email e partite salvate. Attenzione: riporta anche la mano dominante a destra.
- Le impostazioni restano salvate tra una partita e l'altra. Dopo la partita il pulsante **TORNA AL MENU** riporta al menu senza perdere nulla.
- **Indizi di profondità:** facili = ombra, grandezza prospettica, pavimento a punti. Difficili = grandezza angolare costante, niente ombre né pavimento; con la caduta il terreno è una fascia uniforme a livello fisso e la velocità di caduta è angolare, per non regalare indizi di profondità. Si registra sempre quali.

## 6. Suoni

Tre gruppi separati (toni; le voci registrate si aggiungono quando ci sono i file):

1. **Esito** (predefinito acceso): giusto, troppo presto, mancata (omissione), palloncino colpito, palloncino a terra, ciascuno con un suono diverso.
2. **Apparizione dell'ape** (predefinito spento).
3. **Segnale rosso** (predefinito **spento**). **Attenzione:** se lo accendi, il giocatore può rispondere al suono **senza guardare l'ape**; il tempo di reazione in quel caso non misura più la vista. Lo si accende solo per capire se aiuta chi non vede bene il rosso.

Nessuna vibrazione (non disponibile nel visore).

## 7. Prova audio (da fare prima)

Nella pagina e nel menu VR c'è la **Prova audio** con le **12 voci**: per ognuna la frase prevista, se il file è caricato e decodificato, la durata e un pulsante ▶. Le voci 01-07 sono quelle del gioco 2; le 08-12 sono quelle del gioco 1 (08 regola all'inizio, 09 "Rossa! Colpiscila!" solo con il suono del segnale, 10 troppo presto, 11 omissione, 12 ape colpita).

**Le voci 08-12 non sono ancora state registrate**: nella Prova audio compaiono come "file non caricato" e il gioco 1 usa i **toni**. Appena i file ci sono (nome che comincia con il numero) si preparano con lo script e si ripubblica.

## 8. Cosa misura il gioco (e cosa NO)

- Il gioco 1 allena **inseguimento di vergenza e tempismo**: l'ape che si avvicina chiede una convergenza crescente e il giocatore deve rispondere solo quando diventa rossa.
- **Il raggio colpisce per direzione**, quindi la profondità non è necessaria per centrare i bersagli: il gioco non dimostra che il giocatore usa la stereopsi.
- L'ape colpita con la **mano non dominante** può avere tempi più lenti per **motivi motori e non solo visivi**: i tempi di reazione dell'ape non vanno letti come puro dato visivo.
- La **velocità adattiva** rende le sedute **confrontabili solo con la velocità costante**: con l'adattiva la difficoltà cambia durante la seduta e i punteggi non sono confrontabili. Con il **tetto A** la velocità resta tra il minimo e V0; con il **tetto B** può salire oltre V0 fino alla massima, quindi due sedute con tetto, massima, N, M o gradino diversi **non sono confrontabili** tra loro (si registrano tutti questi valori, la velocità massima raggiunta e la lista dei cambi).
- Il numero di palloncini e il loro fattore di riduzione cambiano la difficoltà (più palloncini e più piccoli): anche questi sono registrati.
- Il tempo di reazione è misurato dal primo fotogramma in cui l'ape è rossa fino al grilletto (precisione di un fotogramma, circa 14-28 ms); non comprende i ritardi del visore e del controller.

## 9. Dati e risultati

I risultati compaiono nella pagina dopo la partita (riepilogo e tabelle dei due giochi), si possono mandare per email, copiare o scaricare. Si salvano solo sul dispositivo, in una chiave separata da quella del Visore; ogni partita porta l'id del gioco (`ape_rossa` oppure `ape_e_palloncino`). Per il gioco 1 si registrano, tra l'altro: modalità, compiti, mano per compito, indizi, limite, durata; per i palloncini velocità di partenza, tetto (A o B), velocità massima impostata e raggiunta, N e M di fila, gradino, minimo, numero di palloncini impostato ed effettivo, fattore di riduzione, velocità di ogni palloncino, tempo dalla comparsa al colpo (medio e DS), profondità, colpiti, caduti a terra, velocità raggiunta (media dell'ultimo minuto) e finale, palloncini a terra durante l'ape e nella finestra rossa; l'**uscita con il tasto laterale**; per l'ape velocità, distanza di partenza, settori di partenza e arrivo, tempo di reazione (medio e DS), anticipi, omissioni, tipo di ape ("avvicinamento").

## 10. Cosa non è stato provato nel Pico vero

- **Novità della v0.2.1 provate solo sul simulatore:** fluidità a 72/90 Hz con 8 palloncini; centratura dei pulsanti «i», − e + con il raggio della pagina nel Pico Browser; leggibilità dei testi nel visore (riga «in uso», cerchio dell'uscita); comfort a velocità alte; **comportamento reale del tasto laterale tenuto 5 secondi** e **se il sistema del Pico intercetta il tasto laterale** (se sì, l'uscita non funziona e si usa B o Y tenuto 2 secondi).

- Il gioco 1 della v0.2 è stato provato da Daniele nel Pico con i valori predefiniti (281 palloncini colpiti e 2 caduti, ape 8 su 8, reazione 619 ms): da lì sono nate le correzioni della v0.2.1. Il gioco 2 è stato provato da Daniele nella v0.1 (audio, profondità e partita di 3 minuti senza problemi).
- Leggibilità del rosso e della pulsazione dell'ape, dei palloncini blu e del terreno; senso di profondità; comfort alla distanza del limite.
- Mira con il raggio sull'ape (area di colpo di 2 gradi) e sui palloncini in caduta; uso delle due mani; `handedness` dei controller veri.
- Se i valori predefiniti (0,25 m/s di caduta, ape ogni 10-20 s a 0,5 m/s, finestra 2,5 s, 4 palloncini) sono giusti per il ragazzo.
- Le voci 08-12 (non esistono ancora) e il volume delle voci nel Pico.

## 11. Cosa guardare nella prossima prova (e cosa mandarmi)

| Domanda | Risposta |
|---|---|
| I pulsanti **i**, − e + si centrano bene con il raggio nel Pico Browser? Le spiegazioni si leggono? | |
| APPLICA: l'avviso giallo compare e il gioco 1 parte solo dopo APPLICA? La riga «IMPOSTAZIONI IN USO» in VR si legge? | |
| Con tetto B e massima 1,0 la velocità sale oltre 0,25? A che velocità il giocatore comincia a sbagliare? A quale non riesce più a colpire (3 m/s? di più?)? | |
| Con N = 8 e M = 4 la velocità cambia in modo sensato? Una caduta isolata non fa più scendere? | |
| Con 6 o 8 palloncini il gioco è fluido (nessuno scatto)? I palloncini restano distinti e abbastanza grandi per vederli e colpirli? Quanto è il fattore di riduzione scritto nei risultati? | |
| **Tasto laterale** tenuto 5 secondi: il cerchio compare e si riempie? La partita si interrompe, si salva e si torna al menu dei giochi con il messaggio? **Oppure il sistema del Pico intercetta il tasto** (compare un menu di sistema)? Funziona con tutte e due le mani, anche in pausa? | |
| B o Y tenuto 2 secondi ferma ancora la partita con il riepilogo? | |
| Il rosso dell'ape, la pulsazione, le direzioni, la finestra di 2,5 s, i suoni: come nella prima prova? C'è disagio, mal di testa o visione doppia? | |
| Riepilogo dalla pagina (email o foto), con velocità massima raggiunta e palloncini effettivi | |
