# SFDN Gioco v0.2 · Ape rossa e Ape e palloncino

**Istruzioni brevi per l'operatore**

_Ottica Stefanucci, Sinalunga · 3 novembre 2026_

**Sperimentale: non è un trattamento validato.** Sessioni brevi e **con supervisione**. **Interrompi subito** se compaiono disagio, mal di testa o visione doppia (B o Y tenuto 2 secondi, oppure togli il visore).

## 1. Come si apre

1. Nel browser del Pico apri `https://daziele74.github.io/sfdn-visore/gioco/`.
2. Nella pagina scrivi il nome (se in questo browser hai già usato il Visore, il nome e la soglia stereo si leggono da lì, senza modificarli).
3. Scegli le impostazioni. Per la prima prova lascia quelle predefinite: **limite vicino medio 1,5 m, 3 minuti, indizi facili, mano dominante destra, voce sì**.
4. Premi **ENTRA IN VR**. Il primo menu in VR fa scegliere: **1 APE ROSSA** oppure **2 APE E PALLONCINO** (più PROVA AUDIO ed ESCI).

## 2. Gioco 1 · APE ROSSA

**Regola fissa: il rosso vuol dire sempre "colpisci ora".** Il rosso è riservato all'ape: nessun altro oggetto è rosso. Il segnale è rosso **più pulsazione** (l'ape si ingrandisce e rimpicciolisce e cambia tonalità), così si riconosce anche senza distinguere bene i colori.

- **Palloncini blu**, da 3 a 5 insieme (predefinito 4), a distanze diverse tra il limite vicino e circa 5 m. Si colpiscono con la **mano dominante** (predefinita destra), con il raggio e il grilletto.
- **A caduta** (predefinito): scendono in verticale a velocità costante e vanno colpiti **prima che tocchino il terreno** (il terreno si vede). **Fermi**: restano dove sono finché li colpisci. Quando un palloncino è colpito o cade a terra ne compare uno nuovo in un altro punto e a un'altra distanza.
- **L'ape** compare a caso ogni 10-20 secondi. Parte da lontano (circa 5 m) e si avvicina piano (0,5 m/s, con una variazione casuale di circa il 20%). Quando arriva al **limite vicino diventa ROSSA e pulsa** e resta così per **2,5 secondi**: in quel tempo va colpita con l'**altra mano** (la non dominante, predefinita sinistra). Poi se ne va con una breve dissolvenza.
  - Colpo **prima** del rosso: **"troppo presto"**. Nessuna penalità di punti.
  - Colpo nella finestra rossa: **giusto**; si misura il tempo di reazione dal momento in cui diventa rossa.
  - Nessun colpo: **omissione**, perdi 1 punto.
- Ogni volta l'ape cambia **direzione di partenza e di arrivo** (settori diversi da quelli degli ultimi due passaggi). Non va mai verso il viso e nessun punto del suo percorso è più vicino del limite scelto.
- **Ogni raggio colpisce solo il suo bersaglio.** Un colpo con la mano dei palloncini sull'ape, o con la mano dell'ape su un palloncino, è ignorato e registrato (nessuna penalità). I due raggi hanno colori diversi (viola per i palloncini, verde chiaro per l'ape); nessuno è rosso.
- **Punti:** palloncino colpito +1, ape colpita +5, omissione -1 (mai sotto zero).
- **Velocità adattiva** (predefinita, solo palloncini a caduta): la velocità di partenza V0 è anche il tetto. Dopo **4 palloncini a terra** scende di un gradino (15% di V0); dopo **8 colpiti** risale di un gradino, mai oltre V0; non scende sotto il 30% di V0. I contatori sono cumulativi e si azzerano a ogni cambio. Si può scegliere la velocità costante. La velocità corrente è scritta in piccolo sul tabellone (per l'operatore; si può togliere dalle AVANZATE).
- **Compiti:** "palloncini + ape" (predefinito), "solo palloncini", "solo ape". **Una mano sola:** un solo raggio colpisce palloncini e ape. Se c'è un solo controller fa tutto lui. Per i mancini si sceglie "sinistra" come mano dominante.

## 3. Gioco 2 · APE E PALLONCINO

È il gioco della versione 0.1, **invariato**: 5 palloncini a distanze diverse; l'ape vola verso il più vicino e si posa; il giocatore lo colpisce quando l'ape è sopra. Colpo con l'ape in volo = "troppo presto"; altro palloncino = errore; se non lo colpisce entro la sosta (2 secondi) l'ape lo fa scoppiare (-1 punto). Impostazioni proprie nella pagina: facilitazione colore, sosta, volo.

## 4. Tasti (uguali nei due giochi)

| Tasto | Cosa fa |
|---|---|
| Grilletto | Colpisce, e preme i pulsanti dei menu |
| A o X (breve) | Pausa e ripresa. Nel gioco 1 il passaggio dell'ape interrotto non conta |
| B o Y tenuto 2 secondi | Ferma la partita |

## 5. Impostazioni (pagina, fuori dalla VR)

- **Comuni ai due giochi:** nome, mano dominante, limite vicino (facile 2,5 m, medio 1,5 m, impegnativo 0,8 m, libero da 0,4 a 6 m), durata (1-10 minuti), indizi (facili o difficili), voce, email dei risultati.
- **Gioco 1, BASE:** compiti, palloncini (caduta o fermi), velocità adattiva sì/no, tre gruppi di suoni.
- **Gioco 1, AVANZATE (riquadro chiuso):** numero di palloncini, velocità V0, gradino, soglie (4 a terra / 8 colpiti), minimo, velocità sul tabellone, intervallo di comparsa dell'ape, velocità e variazione dell'ape, finestra rossa, area di colpo, campo comodo, settori, una mano sola.
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
- La **velocità adattiva** rende le sedute **confrontabili solo con la velocità costante**: con l'adattiva la difficoltà cambia durante la seduta e i punteggi non sono confrontabili.
- Il tempo di reazione è misurato dal primo fotogramma in cui l'ape è rossa fino al grilletto (precisione di un fotogramma, circa 14-28 ms); non comprende i ritardi del visore e del controller.

## 9. Dati e risultati

I risultati compaiono nella pagina dopo la partita (riepilogo e tabelle dei due giochi), si possono mandare per email, copiare o scaricare. Si salvano solo sul dispositivo, in una chiave separata da quella del Visore; ogni partita porta l'id del gioco (`ape_rossa` oppure `ape_e_palloncino`). Per il gioco 1 si registrano, tra l'altro: modalità, compiti, mano per compito, indizi, limite, durata; per i palloncini velocità iniziale, tetto, velocità di ogni palloncino, tempo dalla comparsa al colpo (medio e DS), profondità, colpiti, caduti a terra, velocità raggiunta (media dell'ultimo minuto) e finale, palloncini a terra durante l'ape e nella finestra rossa; per l'ape velocità, distanza di partenza, settori di partenza e arrivo, tempo di reazione (medio e DS), anticipi, omissioni, tipo di ape ("avvicinamento").

## 10. Cosa non è stato provato nel Pico vero

- Tutto il gioco 1 (provato solo sul simulatore). Il gioco 2 è stato provato da Daniele nella v0.1 (audio, profondità e partita di 3 minuti senza problemi).
- Leggibilità del rosso e della pulsazione dell'ape, dei palloncini blu e del terreno; senso di profondità; comfort alla distanza del limite.
- Mira con il raggio sull'ape (area di colpo di 2 gradi) e sui palloncini in caduta; uso delle due mani; `handedness` dei controller veri.
- Se i valori predefiniti (0,25 m/s di caduta, ape ogni 10-20 s a 0,5 m/s, finestra 2,5 s, 4 palloncini) sono giusti per il ragazzo.
- Le voci 08-12 (non esistono ancora) e il volume delle voci nel Pico.

## 11. Cosa guardare nella prima prova del gioco 1 (e cosa mandarmi)

| Domanda | Risposta |
|---|---|
| Il rosso dell'ape si nota subito? La pulsazione si vede anche senza il colore? | |
| L'ape arriva da direzioni diverse? Dà fastidio quando arriva vicino al limite (1,5 m)? Visione doppia? | |
| I palloncini blu si vedono bene vicino e lontano? Il terreno si vede? La profondità sembra naturale? | |
| La caduta (0,25 m/s) è troppo lenta o troppo veloce? Quanti palloncini cadono a terra in 3 minuti? | |
| La velocità adattiva scende e risale in modo sensato? (guarda il numero sul tabellone) | |
| Mano dominante per i palloncini e altra mano per l'ape: comodo? Si confondono i raggi? Colpi ignorati (tipo sbagliato) frequenti? | |
| Il raggio colpisce bene l'ape e i palloncini in caduta? Serve un'area di colpo più grande? | |
| La finestra rossa di 2,5 s è giusta? Troppi "troppo presto" o troppe omissioni? | |
| Quando arriva l'ape il giocatore lascia cadere i palloncini (palloncini a terra durante l'ape)? | |
| I suoni di esito sono chiari? Prova poi apparizione e segnale (solo per capire). Le voci 01-07 vanno ancora bene? | |
| Pausa (A/X) e stop (B/Y 2 s) funzionano? Il riepilogo arriva per email? | |
| Riepilogo dalla pagina (email o foto) | |
