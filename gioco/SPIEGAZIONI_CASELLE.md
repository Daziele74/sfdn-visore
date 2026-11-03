# Spiegazioni delle caselle (SFDN Gioco v0.2.1)

Questa è l'**unica fonte** dei testi del pulsante **i**: `tools/build_gioco.py` li copia nella pagina del gioco. Se li cambi qui, basta rifare la costruzione (stage 03) e il rilascio (stage 05).

Come sono scritti: per un bambino di 10 anni. Ogni casella ha quattro parti: **Cosa fa**, cosa succede se la **alzi** (o se scegli una cosa), cosa succede se la **abbassi** (o se scegli l'altra), e un **Esempio** concreto. Le caselle con una scelta (menu a tendina) spiegano le due scelte.

Formato (non cambiarlo, serve alla costruzione): ogni casella comincia con `## id | titolo`, poi righe `**Etichetta.** testo`.

---

## sNome | Nome o codice
**Cosa fa.** Serve a scrivere chi sta giocando, così le partite si riconoscono nei risultati.
**Se lo scrivi.** Il nome finisce nei risultati e nella mail, e il gioco ricorda i record di quella persona.
**Se lo lasci vuoto.** Il gioco usa il nome del Visore, se c'è. Altrimenti le partite restano senza nome.
**Esempio.** Scrivi un codice come «A12». Meglio un codice che il nome vero, se vuoi proteggere la privacy.

## sMano | Mano dominante
**Cosa fa.** Dice qual è la mano che il giocatore usa meglio, quella con cui scrive.
**Se scegli destra.** Nel gioco 1 i palloncini si colpiscono con la mano destra e l'ape con la sinistra. Nel gioco 2 colpisce la destra.
**Se scegli sinistra.** Si scambiano le mani: i palloncini con la sinistra, l'ape con la destra.
**Esempio.** Un bambino mancino sceglie «sinistra», così la mano forte fa il lavoro più frequente, cioè i palloncini.

## sProfilo | Profilo del limite vicino
**Cosa fa.** È una scorciatoia per scegliere quanto vicino possono arrivare gli oggetti agli occhi: facile, medio o impegnativo.
**Se vai verso «facile».** Gli oggetti restano lontani (2,5 metri): occhi più rilassati, meno fatica.
**Se vai verso «impegnativo».** Gli oggetti arrivano più vicini (0,8 metri): gli occhi devono girare di più verso il naso, è più faticoso.
**Esempio.** Per la prima volta si parte da «medio» (1,5 metri). «Valore libero» si usa quando scrivi tu i metri nella casella accanto.

## sNear | Limite vicino
**Cosa fa.** Dice quanti metri al minimo devono restare tra gli occhi e qualsiasi oggetto del gioco. Nessun oggetto lo supera mai.
**Se lo alzi.** Gli oggetti restano più lontani: gioco più comodo, ma anche meno allenante.
**Se lo abbassi.** Gli oggetti arrivano più vicino: gli occhi lavorano di più, ma si può sentire fatica o vedere doppio.
**Esempio.** Con 1,5 l'ape si ferma a un metro e mezzo dal naso. Con 0,8 si ferma quasi a un braccio di distanza.

## sDur | Durata della partita
**Cosa fa.** Sceglie quanto dura la partita, con i pulsanti 30 secondi, 1, 2, 3, 5 o 10 minuti.
**Se scegli più tempo.** La partita è più lunga: più palloncini e più passaggi dell'ape, ma gli occhi si stancano di più.
**Se scegli meno tempo.** La partita è corta: va bene per provare o per chi si stanca presto.
**Esempio.** Per provare un'impostazione nuova bastano 30 secondi. Per una partita vera si parte da 3 minuti.

## sIndizi | Indizi di profondità
**Cosa fa.** Decide quanti aiuti ci sono per capire quanto è lontano un oggetto.
**Se scegli «facili».** Ci sono ombre, un pavimento a puntini e gli oggetti lontani sembrano più piccoli, come nella vita vera.
**Se scegli «difficili».** Tutti gli oggetti sembrano grandi uguale e non ci sono ombre né pavimento: per capire la distanza bisogna usare davvero i due occhi.
**Esempio.** Con «facili» capisci che un palloncino è lontano perché è piccolo. Con «difficili» non lo capisci dalla grandezza.

## sVoce | Voce
**Cosa fa.** Accende o spegne le frasi registrate («Bravo!», «Troppo presto!»).
**Se scegli «sì».** Si sentono le frasi quando i file audio ci sono. Se un file manca si sente un suono semplice.
**Se scegli «no».** Si sentono solo suoni semplici, senza parole.
**Esempio.** Per un bambino che si distrae con le parole, si può scegliere «no» e lasciare solo i suoni.

## sMail | Email dei risultati
**Cosa fa.** È l'indirizzo a cui preparare la mail con i risultati, quando premi «Invia i risultati per email».
**Se lo scrivi.** La mail si prepara già con quell'indirizzo. Resta solo su questo dispositivo.
**Se lo lasci vuoto.** Il gioco prova a usare l'indirizzo del Visore. Se non c'è, chiede di scriverlo.
**Esempio.** Scrivi l'indirizzo di chi deve leggere i risultati, poi controlli la mail e premi Invia.

## sCompito | Compiti
**Cosa fa.** Sceglie che cosa bisogna fare: solo palloncini, solo ape, oppure tutte e due le cose insieme.
**Se scegli «palloncini + ape».** Si colpiscono i palloncini e, quando l'ape diventa rossa, anche l'ape. È il gioco completo.
**Se scegli «solo palloncini» o «solo ape».** Si fa una cosa sola: più semplice, utile per imparare o per misurare una cosa alla volta.
**Esempio.** Se vuoi vedere solo quanto è veloce a rispondere al rosso, scegli «solo ape».

## sBaMode | Palloncini (a caduta o fermi)
**Cosa fa.** Decide se i palloncini scendono verso il terreno o se restano fermi in aria.
**Se scegli «a caduta».** I palloncini scendono piano e vanno colpiti prima che tocchino il terreno. C'è un po' di fretta.
**Se scegli «fermi».** Restano lì finché non li colpisci: nessuna fretta, e la velocità non conta.
**Esempio.** Per imparare i comandi si usano i palloncini fermi. Per allenarsi sul serio, a caduta.

## sAdatt | Velocità dei palloncini
**Cosa fa.** Dice se la velocità dei palloncini cambia da sola durante la partita.
**Se scegli «adattiva».** Se ne colpisci tanti di fila i palloncini vanno più veloci. Se ne cadono tanti di fila vanno più piano.
**Se scegli «costante».** La velocità non cambia mai, così le partite si possono confrontare fra loro.
**Esempio.** Con «adattiva» il gioco segue il giocatore. Con «costante» lo metti sempre alla stessa prova.

## sEsito | Suoni di esito
**Cosa fa.** Accende o spegne i suoni che dicono come è andata: colpito, a terra, troppo presto, ape giusta.
**Se li accendi.** Ogni cosa ha un suono diverso e il giocatore capisce subito se ha fatto bene.
**Se li spegni.** Il gioco è silenzioso: ci si accorge dell'esito solo guardando.
**Esempio.** Un «pop» quando un palloncino scoppia e un suono basso quando cade a terra.

## sAppar | Suono di apparizione dell'ape
**Cosa fa.** Fa suonare un piccolo suono quando l'ape compare in lontananza.
**Se lo accendi.** Il giocatore sa che l'ape sta arrivando anche se guarda altrove.
**Se lo spegni.** L'ape arriva in silenzio e bisogna accorgersene guardando.
**Esempio.** Se spegni il suono, il giocatore deve tenere gli occhi aperti per vedere l'ape che spunta.

## sSegn | Suono del segnale rosso
**Cosa fa.** Fa suonare un suono nel momento in cui l'ape diventa rossa.
**Se lo accendi.** Il giocatore può rispondere al suono senza guardare l'ape: il tempo di reazione non misura più la vista.
**Se lo spegni.** Si risponde solo vedendo il rosso, e la misura è quella giusta per la vista.
**Esempio.** Si accende solo per capire se un bambino che non vede bene il rosso riesce con un aiuto in più.

## sNBal | Palloncini insieme
**Cosa fa.** Dice quanti palloncini ci sono nello stesso momento, da 3 a 8.
**Se lo alzi.** Ci sono più palloncini da guardare e colpire. Per farli stare tutti si rimpiccioliscono un po', tutti nello stesso modo. Se ancora non ci stanno, il gioco ne usa uno in meno e lo scrive nei risultati.
**Se lo abbassi.** Ce ne sono meno, restano più grandi e il gioco è più facile.
**Esempio.** Con 4 palloncini è come all'inizio. Con 8 è affollato e i palloncini sono più piccoli.

## sRedMax | Riduzione massima
**Cosa fa.** Dice quanto possono rimpicciolirsi i palloncini quando ce ne sono tanti, come percentuale della grandezza normale.
**Se lo alzi.** I palloncini si rimpiccioliscono meno. Se non ci stanno, il gioco usa più spesso un palloncino in meno.
**Se lo abbassi.** I palloncini possono diventare molto piccoli per far stare tutti, e sono più difficili da vedere.
**Esempio.** Con 60 i palloncini possono ridursi fino al 60% della grandezza normale, non di più.

## sV0 | Velocità di caduta V0 (partenza)
**Cosa fa.** È quanto in fretta scendono i palloncini all'inizio, in metri al secondo. È anche il punto da cui parte la velocità adattiva.
**Se la alzi.** Scendono più veloci, come sassi. Sopra circa 3 metri al secondo quasi non si riesce più a colpirli.
**Se la abbassi.** Scendono più piano, come foglie.
**Esempio.** Con 0,25 hai tempo di sistemarti. Con 2 devi essere molto pronto.

## sTetto | Tetto della velocità
**Cosa fa.** Dice se la velocità può salire oltre quella di partenza.
**Se scegli «B».** Se il giocatore è bravo la velocità sale anche oltre V0, fino alla velocità massima. Serve a cercare il limite vero.
**Se scegli «A».** La velocità non supera mai V0: può solo scendere e tornare a V0.
**Esempio.** Con V0 uguale a 0,25 e tetto B, un giocatore bravo può arrivare fino a 1 metro al secondo. Con tetto A resta a 0,25 al massimo.

## sVMax | Velocità massima (tetto B)
**Cosa fa.** È il limite più alto che la velocità può raggiungere con il tetto B, in metri al secondo.
**Se la alzi.** I palloncini possono diventare molto veloci. Il gioco non mette un limite finto: si vede dove il giocatore non ce la fa più.
**Se la abbassi.** La velocità smette di salire prima. Se la metti sotto V0, vale V0 e il gioco lo scrive accanto alla casella.
**Esempio.** Con massima 1 la velocità arriva al massimo a 1 metro al secondo, anche se il giocatore è bravissimo.

## sVStep | Gradino di velocità
**Cosa fa.** Dice di quanto cambia la velocità a ogni salita o discesa, come percentuale di V0.
**Se lo alzi.** La velocità fa salti grandi: il gioco si adatta in fretta ma meno dolcemente.
**Se lo abbassi.** I salti sono piccoli e la velocità cambia piano piano.
**Esempio.** Con V0 uguale a 1 e gradino 15, ogni cambio sposta la velocità di 0,15 metri al secondo.

## sNUp | Sale dopo N colpiti di fila
**Cosa fa.** Dice quanti palloncini consecutivi bisogna colpire, senza farne cadere nessuno, perché la velocità salga di un gradino.
**Se lo alzi.** Bisogna essere bravi più a lungo prima di andare più veloci: la velocità sale più di rado.
**Se lo abbassi.** Basta poco per andare più veloci: la velocità sale spesso.
**Esempio.** Con 8, se colpisci 8 palloncini senza farne cadere neanche uno, la velocità sale. Se uno cade, si ricomincia a contare.

## sNDown | Scende dopo M a terra di fila
**Cosa fa.** Dice quanti palloncini consecutivi devono cadere a terra, senza colpirne nessuno, perché la velocità scenda di un gradino.
**Se lo alzi.** Il gioco aspetta di più prima di rallentare: il giocatore resta in difficoltà più a lungo.
**Se lo abbassi.** Il gioco rallenta presto, dopo poche cadute.
**Esempio.** Con 4, se cadono 4 palloncini uno dopo l'altro la velocità scende. Una caduta sola, in mezzo a tanti colpiti, non fa scendere nulla.

## sVMin | Velocità minima
**Cosa fa.** È il limite più basso a cui può scendere la velocità, come percentuale di V0.
**Se lo alzi.** La velocità non scende troppo: il gioco resta più sfidante anche per chi sbaglia.
**Se lo abbassi.** La velocità può diventare molto lenta, per aiutare chi fa fatica.
**Esempio.** Con V0 uguale a 1 e minimo 30, i palloncini non vanno mai più piano di 0,3 metri al secondo.

## sShowV | Velocità sul tabellone
**Cosa fa.** Decide se scrivere in piccolo, sul tabellone, la velocità dei palloncini in questo momento.
**Se scegli «sì».** L'operatore può leggerla durante la partita, ma anche il giocatore la vede.
**Se scegli «no».** Il giocatore non vede il numero e non si distrae. La velocità si legge poi nei risultati.
**Esempio.** Se il giocatore si agita vedendo il numero salire, conviene scegliere «no».

## sApeMin | Compare ogni, almeno
**Cosa fa.** È il tempo minimo, in secondi, che passa tra la fine di un passaggio dell'ape e l'arrivo del successivo.
**Se lo alzi.** L'ape si fa vedere di rado: più tempo per i palloncini e meno occasioni di rispondere.
**Se lo abbassi.** L'ape torna presto: più passaggi in una partita.
**Esempio.** Con 10 e massimo 20, l'ape arriva ogni 10 fino a 20 secondi, scelti a caso.

## sApeMax | Compare ogni, al massimo
**Cosa fa.** È il tempo massimo, in secondi, tra un passaggio dell'ape e il successivo. Non può essere minore del minimo.
**Se lo alzi.** Ci sono pause più lunghe e imprevedibili tra un'ape e l'altra.
**Se lo abbassi.** I tempi diventano più regolari e l'ape si fa vedere più spesso.
**Esempio.** Se minimo e massimo sono uguali, l'ape arriva sempre alla stessa distanza di tempo.

## sApeVel | Velocità di avvicinamento
**Cosa fa.** Dice quanto in fretta l'ape si avvicina, in metri al secondo.
**Se la alzi.** L'ape arriva svelta: gli occhi devono girare verso il naso più in fretta, ed è più difficile.
**Se la abbassi.** L'ape arriva piano, e c'è più tempo per prepararsi.
**Esempio.** Con 0,5 l'ape percorre cinque metri in dieci secondi. Con 1 ci mette la metà.

## sApeVar | Variazione casuale
**Cosa fa.** Cambia un po', a caso, la velocità dell'ape e la distanza da cui parte, così non è sempre uguale.
**Se la alzi.** Ogni passaggio è più diverso dagli altri e meno prevedibile.
**Se la abbassi.** I passaggi si somigliano di più. A zero sono tutti uguali.
**Esempio.** Con 20 per cento, un'ape che dovrebbe andare a 0,5 metri al secondo può andare tra 0,4 e 0,6.

## sApeWin | Finestra rossa
**Cosa fa.** È il tempo, in secondi, in cui l'ape resta rossa e si può colpire.
**Se la alzi.** C'è più tempo per rispondere: più facile, meno omissioni.
**Se la abbassi.** C'è poco tempo e bisogna essere pronti: più difficile.
**Esempio.** Con 2,5 secondi hai il tempo di mirare. Con 1 secondo devi colpire quasi subito.

## sApeAng | Area di colpo minima dell'ape
**Cosa fa.** Dice quanto grande è la zona intorno all'ape in cui il raggio la colpisce, misurata in gradi di visione.
**Se la alzi.** Il raggio colpisce l'ape anche se la manca un po': più facile, anche per mani poco ferme.
**Se la abbassi.** Bisogna mirare con più precisione.
**Esempio.** Con 2 gradi la zona è larga circa quanto due dita tenute a braccio teso.

## sFAz | Campo comodo, orizzontale
**Cosa fa.** Dice quanto a destra e a sinistra, in gradi, possono comparire palloncini e ape.
**Se lo alzi.** Gli oggetti possono stare più lontano ai lati: bisogna girare di più la testa o gli occhi.
**Se lo abbassi.** Gli oggetti stanno più al centro, davanti a te.
**Esempio.** Con 30 gradi, a due metri di distanza gli oggetti stanno in una fascia larga più di due metri.

## sFEl | Campo comodo, verticale
**Cosa fa.** Dice quanto in alto e in basso, in gradi, possono comparire palloncini e ape.
**Se lo alzi.** Gli oggetti arrivano più in alto: bisogna alzare lo sguardo.
**Se lo abbassi.** Gli oggetti restano più vicini all'altezza degli occhi.
**Esempio.** Con 20 gradi non devi mai guardare troppo in su, e il collo non si stanca.

## sSecAz | Settori in orizzontale
**Cosa fa.** Divide il campo in tante strisce da sinistra a destra. L'ape cambia ogni volta striscia di partenza e di arrivo.
**Se lo alzi.** Ci sono più strisce, più direzioni diverse, e l'ape è più imprevedibile.
**Se lo abbassi.** Ci sono meno direzioni e l'ape si ripete più spesso.
**Esempio.** Con 4 strisce e 2 file ci sono 8 settori. L'ape non usa quelli degli ultimi due passaggi.

## sSecEl | Settori in verticale
**Cosa fa.** Divide il campo in file dall'alto al basso. Insieme alle strisce dà il numero dei settori.
**Se lo alzi.** Ci sono più file: l'ape può arrivare da più altezze diverse.
**Se lo abbassi.** Meno altezze diverse, ape più prevedibile.
**Esempio.** Con 1 fila l'ape arriva sempre più o meno all'altezza degli occhi. Con 2 file, a volte più in alto e a volte più in basso.

## sUna | Una mano sola
**Cosa fa.** Dice se si gioca con un solo controller, che colpisce sia i palloncini sia l'ape.
**Se scegli «sì».** Un solo raggio fa tutto. L'ape ha la precedenza se il raggio è sull'ape.
**Se scegli «no».** Servono due mani: una per i palloncini e l'altra per l'ape.
**Esempio.** Se un bambino riesce a usare bene una mano sola, si sceglie «sì».

## sColore | Facilitazione colore (gioco 2)
**Cosa fa.** Nel gioco 2 può colorare di azzurro il palloncino più vicino, per aiutare a trovarlo.
**Se scegli «accesa».** Il palloncino più vicino è azzurro e gli altri sono rossi: l'aiuto è grande.
**Se scegli «spenta».** Tutti i palloncini sono rossi e bisogna capire da soli qual è il più vicino.
**Esempio.** Si accende all'inizio per imparare, poi si spegne per allenarsi davvero.

## sStay | Sosta dell'ape sul palloncino (gioco 2)
**Cosa fa.** Nel gioco 2 è il tempo, in secondi, in cui l'ape sta posata sul palloncino prima di farlo scoppiare.
**Se lo alzi.** C'è più tempo per colpire il palloncino: più facile.
**Se lo abbassi.** L'ape scoppia il palloncino presto: bisogna essere veloci.
**Esempio.** Con 2 secondi hai il tempo di mirare. Con 0,5 devi colpire quasi subito.

## sFlight | Volo dell'ape (gioco 2)
**Cosa fa.** Nel gioco 2 è il tempo, in secondi, che l'ape impiega a volare fino al palloncino.
**Se lo alzi.** L'ape vola più piano e c'è più tempo per capire dove andrà.
**Se lo abbassi.** L'ape vola più in fretta e arriva subito.
**Esempio.** Con 4 secondi l'ape ci mette un po'. Con 2 arriva quasi di colpo.
