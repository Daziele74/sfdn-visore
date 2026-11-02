# SFDN · Visore v0.6.1

**Istruzioni per la prova (novità rispetto alla v0.5D)**

_Saccadic Fixator de Noialtri · Ottica Stefanucci, Sinalunga · 2 novembre 2026_

Valgono le istruzioni precedenti. **Tutto è sperimentale e non dà indicazioni cliniche.** Se compaiono nausea, mal di testa o visione doppia fastidiosa, ferma la seduta.

Questa è la **tappa 1** della v0.6: solo correzioni. Il modulo "Riserve fusionali" non c'è ancora (arriva dalla tappa 2).

## 1. Cosa cambia

- **Vibrazione corretta.** Il programma prova prima il metodo `playEffect('dual-rumble')` e, se non va, il vecchio metodo `pulse`.
- **Prova tasti, nuovo riquadro in basso:** scrive quali interfacce di vibrazione trova il visore (`vibrationActuator` sì/no, `hapticActuators` sì/no, per ogni controller) e quale metodo è stato usato per l'ultima vibrazione, con l'eventuale errore.
- **Prova tasti, nuovo pallino:** "CLIC JOYSTICK (pulsante 3)", separato dal pallino del movimento del joystick.
- **Il pulsante "Torna al menu"** della Prova tasti è ora a destra dei pallini.
- **Email:** il campo dell'indirizzo è passato nelle **impostazioni** (riquadro 3, "Email dei risultati"). Si scrive una volta per browser. Un indirizzo già salvato resta.
- Tutto il resto (test 9, sfere, soglia, dicoptica, scheda soggetto, calibrazione, pulsanti Cancella e Azzera) **non cambia**.

## 2. Come provare la vibrazione

1. Entra in VR, premi **Prova tasti**.
2. Leggi il riquadro in basso **prima** di premere: dice cosa trova il visore.
3. Premi il **grilletto** con la mano destra, poi con la sinistra. Poi gli altri tasti.
4. Per ogni pressione dovresti sentire una **vibrazione breve** nel controller. Rileggi il riquadro: **"ultima vibrazione"** dice `playEffect` (metodo nuovo) o `pulse` (vecchio metodo), oppure `nessuna interfaccia`, con un eventuale errore.
5. Premi anche il **clic del joystick** (premi il joystick come un tasto): deve accendersi il pallino "CLIC JOYSTICK".
6. **Torna al menu**: il riepilogo si salva tra i risultati e nella mail, con le interfacce di vibrazione trovate.

## 3. Email

- Apri il riquadro 3 e scrivi l'indirizzo in **Email dei risultati**. Va fatto **una volta per browser**.
- Con il campo vuoto "Invia i risultati per email" non apre Gmail e ricorda dove scrivere l'indirizzo.

## 4. Cosa non è stato provato nel Pico vero

- **Se la vibrazione parte** con `playEffect` o con `pulse`: il simulatore finto ha solo interfacce inventate, non dice niente sul Pico vero.
- **Cosa riporta il Pico** per `vibrationActuator` e `hapticActuators`.
- Se il **clic del joystick** arriva come pulsante 3 (lo si vede solo nel visore).
- La leggibilità del nuovo riquadro e la posizione del pulsante "Torna al menu".
- Il campo email nelle impostazioni su https (nel simulatore funziona).

## 5. Cosa mandarmi

| Domanda | Risposta |
|---|---|
| Riquadro "Vibrazione": cosa scrive per ogni controller (vibrationActuator, hapticActuators)? | |
| "Ultima vibrazione": playEffect, pulse o nessuna? Con quale errore? | |
| Si sente la vibrazione nei controller? Destro, sinistro? | |
| Il pallino del clic joystick si accende? | |
| Il testo del nuovo riquadro si legge bene? | |
| Campo email nelle impostazioni: si trova e resta salvato? | |

Dalla pagina: **Invia i risultati per email** (la Prova tasti è inclusa).
