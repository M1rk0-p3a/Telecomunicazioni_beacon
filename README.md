# Bluetooth Beacons

I beacon Bluetooth sono dispositivi hardware che trasmettono segnali utilizzando la tecnologia Bluetooth Low Energy (BLE). Permettono a dispositivi come smartphone e tablet di eseguire azioni basate sulla localizzazione, rilevando un identificatore univoco universale (UUID) trasmesso dal beacon.

## Componenti principali

### Hardware
Un beacon Bluetooth include:
- **Microcontrollore** con un chip radio BLE.
- **Batteria**, generalmente a bottone agli ioni di litio (240 mAh - 1000 mAh), di conseguenza molto compatta e con poca capacità, che può durare oltre un anno grazie al basso consumo energetico del BLE. Alcuni modelli utilizzano batterie di tipoogia AA alcaline o possono essere alimentati tramite USB o presa di corrente.

### Firmware
Il firmware del beacon controlla principalmente i seguenti parametri:
- **Potenza di Trasmissione (Tx Power)**: Determina la distanza di copertura del segnale. Un valore alto aumenta il raggio in cui il segnale è visivile ma riduce la durata della batteria in quanto aumenta la richiesta di energia.
- **Intervallo di Advertising**: Frequenza di emissione del segnale. Un intervallo breve (100 ms) aumenta la reattività ma consuma più energia, mentre uno lungo (500 ms) riduce il consumo ma può diminuire la reattività.

## Principali protocolli di beacon

### iBeacon (Apple, 2013)
Utilizza BLE per trasmettere un UUID che permette di identificare la posizione fisica del dispositivo o attivare azioni basate sulla localizzazione. Offre due metodi API:
- **Ranging**: Fornisce stime di prossimità quando l'app è attiva.
- **Monitoring**: Funziona anche se l'app non è in esecuzione, rilevando la presenza del dispositivo nel raggio d'azione.

### Eddystone (Google, 2015)
Progetto open-source compatibile con iOS e Android. Supporta diversi tipi di pacchetti dati:
- **Eddystone-UID** e **Eddystone-URL** per trasmettere identificatori e URL.
- **Eddystone-TLM** per inviare dati sullo stato del beacon, come la durata della batteria.

### AltBeacon (Radius Networks)
Standard aperto con funzionalità simili a iBeacon, ma con un supporto più limitato. Offre 25-28 byte per i dati dell'utente, leggermente superiori ai 20-27 byte di iBeacon.

## Considerazioni sulla durata della batteria
La durata della batteria dipende da:
- **Potenza di trasmissione**.
- **Intervallo di advertising** (ad esempio, 100 ms = 1-3 mesi di autonomia, 900 ms = 2-3 anni).
- **Capacità della batteria**.

## Applicazioni
I beacon Bluetooth trovano applicazione in diversi settori:
- **Commercio al dettaglio**: Offerte speciali e pagamenti mobili.
- **Musei**: Informazioni interattive sugli oggetti esposti.
- **Eventi sportivi**: Navigazione all'interno degli stadi e gestione del pubblico.
- **Altro**: Con la continua diffusione di questa tecnologia si stanno scoprendo sempre più campi d'utilizzo, attualmente è in forte crescita nei settori della sanità e dell'istruzione.


