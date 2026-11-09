# Unità centrale di Neverina

Schemi elettrici per l'Unità Centrale di Neverina, prodotta in giugno 2026 e utilizzata successivamente come *test-bed* per i nuovi progetti del reparto.

## Struttura
Inizialmente, il circuito è stato realizzato a mano su *perf-board* ed è suddiviso in diverse schede:
 - header per il Raspberry Pi
 - *board 1*
 - *board 2*.

Successivamente, il progetto è stato realizzato su PCB; qui sono presenti i file di progettazione della scheda. 

### Prototipo su *perfboard*
In questo caso, tutti i collegamenti presenti nella schematica sono stati realizzati con connettori JST con numero di pin compatibile con quanto indicato; l'unica eccezione è costituita da alcuni breakout (*e.g.* IMU), saldati direttamente alla scheda per esigenze di spazio.

#### *Board 1* 
Scheda di collegamento fra l'header e la *board 2*. Essa alloggia:
 - IMU (breakout GY-BNO055)
 - connettore per igrometro/termometro (breakout DHT22).

#### *Board 2*
Scheda centrale del sistema, contenente:
 - RTC
 - ADC (su base ADS1115) per la lettura del voltaggio delle due celle LiPO - connessioni al BMS per l'alimentazione dell'intero sistema
 - circuito di ingresso per le due celle LiPO.

#### Altri sensori e schede
Oltre alle tre schede indicate, il sistema include
 - GPS (breakout NEO-6M), connesso direttamente all'header
 - Torpedo2, BMS per le celle LiPO
 - igrometro-termometro (breakout DHT22).

### Prototipo su PCB 
I file relativi alla PCB sono
 - ...WIP...
