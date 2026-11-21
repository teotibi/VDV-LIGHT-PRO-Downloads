# VDV_LIGHT PRO

**Regia per spettacoli teatrali su macOS e Windows.** Gestisce cue, audio, video, immagini, testi e luci DMX da un'unica interfaccia. Importa i progetti QLab 5.

<!-- CHANGELOG_START -->
## Cosa c'è di nuovo in v0.3.9.1

VDV_LIGHT PRO — novità della versione 0.3.9.1
Autore: Matteo Tibiletti

Pagina download — versione 0.3.9.1
Questa versione sistema il movimento delle teste mobili (fluidità, calibrazione,
modifica dei keyframe in diretta sul palco 3D e sulle luci vere), rende più
affidabile l'ascolto della console nell'autodetect e aggiunge il Blackout.
Gli show salvati con la 0.3.9 e la 0.3.8 si aprono senza problemi.

Novità rispetto alla 0.3.9

Movimento delle teste mobili: più fluido
- Prima il movimento poteva andare «a scatti» anche con lo stile Fluido: il
  programma aggiornava le luci solo quando qualcos'altro ridisegnava la
  finestra. Ora, finché un cue è in esecuzione, le luci si aggiornano circa
  60 volte al secondo e l'uscita DMX parte circa 44 volte al secondo.
- Quando un valore cambia, il fotogramma DMX parte subito (entro 12 ms) invece
  di aspettare il giro successivo.

Finestra Movimento
- Per ogni testa e per ogni keyframe c'è un menu a tendina con TUTTI i canali
  DMX della testa (indirizzo · nome) e accanto lo slider del canale scelto:
  scala 0-100 % per i canali in percentuale, 0-255 (o 0-65535 per i canali a
  16 bit) per quelli grezzi, con valori interi.
- Accanto a «Il movimento nel tempo» c'è l'anteprima 3D del palco in diretta
  (il frame del movimento è stato ristretto per fargli posto).
- Quando tocchi o cambi un keyframe (A, B, C…) il palco 3D mostra solo quel
  punto, con la testa dove e come sarà lì; il punto precedente è spento. Il
  keyframe in modifica è evidenziato in giallo. Play, ⏮ o lo slider
  dell'anteprima riportano il palco alla vista nel tempo.
- Lo stesso punto va anche alle luci vere collegate («Mostra anche sulle luci
  vere», attivo di default). L'anteprima nel tempo non muove mai le luci vere.

Calibrazione delle teste
- La calibrazione ora vale anche per il palco 3D: Pan e Tilt passano dalla
  stessa regola per le luci vere e per l'anteprima, così il punto che hai
  calibrato come perpendicolare lo è anche nel 3D, e agli estremi la testa 3D
  si ferma dove si ferma quella vera.
- Durante la calibrazione la testa 3D è disegnata perpendicolare dove la stai
  puntando.

Autodetect e DMX
- «Ascolta la console» ora ascolta sia Art-Net sia sACN (E1.31), manda la
  richiesta ai nodi ogni 3 secondi come QLab, e dice quanti pacchetti ha sentito
  e quali nodi Art-Net hanno risposto.
- Se la console è collegata con un normale cavo DMX o con un'interfaccia USB il
  programma non può ascoltarla: serve un nodo Art-Net o sACN. Il messaggio lo dice.
- Nuovo pulsante Blackout (scheda DMX e Autodetect): manda 0 su tutti i 512
  canali di ogni uscita, anche su quelli senza fari. Se una luce resta accesa
  dopo il blackout, la sta comandando un'altra sorgente (la console o un altro
  programma).

Timeline
- La linea rossa è larga 1 px e ha un margine di 20 px sopra e sotto, come in
  QLab; lo zoom ignora valori non positivi.

Regole verificate su QLab (indirizzi delle funzioni in MECHANICS.md)
- Aggiornamento dei cue in esecuzione, ritrasmissione Art-Net (0,7 s / 0,8 s),
  scadenza dei nodi (10 s), scala degli slider dei parametri, arrotondamento dei
  valori prima che vadano alle luci.

Cosa non c'è (ancora)
- L'ascolto della console non legge il DMX da un cavo o da un'interfaccia USB.
- Il numero «build» resta 309 (come la 0.3.9): il quarto numero della versione
  non lo cambia.

Riepilogo della 0.3.9 (rispetto alla 0.3.8)

Sequenze
- Una sequenza ora contiene i suoi cue: trascina un cue sulla parte bassa della
  riga della sequenza, oppure tra due righe al suo interno, per inserirlo.
- Con più cue selezionati, «Aggiungi › Sequenza» li mette automaticamente dentro
  una nuova sequenza, al posto del primo cue selezionato.
- Un nuovo cue creato con una sequenza selezionata finisce dentro la sequenza;
  se è selezionato un cue già dentro, il nuovo va subito dopo di lui.
- Una sequenza non può essere spostata dentro sé stessa. Ogni spostamento è un
  solo passo di «Annulla».
- Durata della sequenza: il più lungo dei cue (insieme) o la somma (uno dopo
  l'altro). Una sequenza vuota mostra «vuota · trascina qui i cue».

Timeline dal vivo durante la riproduzione
- La linea rossa della timeline avanza in tempo reale mentre la sequenza suona,
  sia che parta con GO, con il pulsante Play o con un trigger; si ferma in pausa.
- Play, Pausa e Stop agiscono su tutti i cue della sequenza.
- I blocchi dei cue si spostano e si ridimensionano con il mouse, con aggancio
  a inizio/fine degli altri cue entro 8 pixel. Zoom con cursore o pizzico.
- La finestra della timeline segue il cue selezionato; «Stacca» o Cmd+< la
  riporta in primo piano senza aprirne una seconda.

Teste mobili
- Movimenti di Pan e Tilt rivisti: sono più fluidi e restano coerenti con
  l'anteprima 3D, la calibrazione e le posizioni salvate.

Riepilogo della 0.3.8 (rispetto alla 0.3.7)

Mixer (pulsante «Mixer» accanto a Keypad, oppure Cmd+Maiusc+M)
- Nuovo mixer luci virtuale, con il pannello del Showtec SM-16/2 FX: Fixture A/B,
  Playback Page 1-5, Record, Copy, Delete, Time, Shape, Setup, Blackout,
  16 Unit, 16 cursori, display LCD, tasti A/B, Exit / Giù / Su / Enter / Clear
  e le due manopole A e B.
- Lavora sui fari dello show: quello che fai si vede subito sulle luci, sulle
  uscite DMX e sul palco 3D.
- Premi un'Unità per scegliere il faro: i 16 cursori muovono i suoi canali
  (Page A = canali 1-16, Page B = 17-32) e le manopole A / B muovono Pan e Tilt.
  Senza Unità scelte i cursori sono i playback e le manopole sono Speed e Fade.
- Playback: 5 pagine da 16 memorie. Record › Unità salva la scena; Copy copia;
  Delete elimina. Se lo stesso canale è in più playback vince il valore più alto.
- Sequenze: con Shape acceso, Record aggiunge un passo (fino a 240). Velocità da
  0,1 secondi a 10 minuti, dissolvenza tra i passi, tocca 3 volte Time per
  impostare il tempo.
- Blackout: tutte le luci a zero senza toccare Pan, Tilt e gli altri canali.
- Setup (menu sul display, con Su / Giù / Enter / Exit): valori in % oppure
  0-255, MIDI acceso o spento, canale MIDI, dissolvenza su tutti i canali o solo
  Pan e Tilt, sequenze automatiche o a mano, inversione di un canale,
  azzeramento del mixer.
- MIDI (se acceso in Setup): le note 0-79 avviano i playback, 120-125 le sequenze,
  126 il blackout, sul canale scelto.
- Clear: libera i valori messi a mano sulle Unità scelte; senza Unità porta a
  zero tutti i playback.
- «Assegna le Unità ai fari» (in fondo alla finestra): scegli quale faro risponde
  a ogni Unità, oppure Automatico per seguire l'ordine dei fari.
- Memorie, assegnazioni e opzioni si salvano con lo show.
- Cmd+< passa anche dal mixer, e una finestra già aperta torna in primo piano.

Cursori più facili da usare
- Le levette dei cursori sono molto più grandi (barrette orizzontali, come sul
  mixer vero) e la guida si colora fino alla levetta, così si vede subito quanto
  è alzato ogni cursore.

Dentro il programma
- Aiuto › «Novità di questa versione» mostra queste note.
- Regole prese dal programma originale (QLab) per i cursori, gli indirizzi dei
  canali a 16 bit e le note di rilascio, con gli indirizzi delle funzioni in
  MECHANICS.md.

Cosa non c'è (ancora)
- Modalità Music (sequenze comandate dal microfono del mixer).
- Cambiare il modello di mixer da foto e manuale: non è previsto. Il mixer è
  fissato sul pannello SM-16/2 FX. Un'idea per il futuro è una finestra
  «Mixer personalizzato» dove si scrive quanti cursori e unità ha.
- Dove la foto del FX non basta, le funzioni seguono il manuale dell'SM-16/2:
  alcune assegnazioni (per esempio le manopole e il tasto Time) sono una
  stima e vanno provate con il mixer vero.

Riepilogo della 0.3.7 (nuovo rispetto alla 0.3.5)
- Calibrazione delle teste mobili: anteprima 3D collegata a Pan e Tilt, partenza
  dalla posizione salvata, posizione «0» salvata anche nei preset, scorrimento a
  due dita sul quadratino Pan/Tilt.
- Scorciatoie: nuovi comandi «Nuovo cue …» per ogni tipo di cue (già assegnati
  Cmd+Maiusc+A / F / V / L / W); il tasto rapido di un cue rifiuta Cmd, Tab,
  Invio e frecce, e Cancella lo toglie.
- Cmd+< passa da una finestra all'altra: finestra principale, finestre aperte,
  di nuovo la principale (con Maiusc si torna indietro).
- Regole verificate su QLab: dissolvenze audio a coseno, durate, scelta di un
  solo file per il Target, trigger MIDI, schermo di uscita, secondo GO ignorato.
- Versione mostrata nel menu File e in «Info».

Pacchetti
- Nuovi pacchetti 0.3.9.1: per Mac due dischi (.dmg), uno per i Mac con chip Apple
  (arm64) e uno per i Mac Intel (x86_64); per Windows lo .zip. Tutti con queste note.
- Per aggiornare: sostituisci la vecchia app con quella nuova. Gli show salvati,
  la libreria dei fari e le impostazioni non vengono cancellati.

<!-- CHANGELOG_END -->

## Ricevi gli aggiornamenti via email

Iscriviti per ricevere un messaggio quando viene pubblicata una nuova versione, con il numero della release, l’elenco delle novità e il link diretto alla pagina ufficiale dei download. Puoi annullare l’iscrizione in qualsiasi momento dal link presente in ogni email.

[Iscriviti agli aggiornamenti di VDV_LIGHT PRO](https://buttondown.com/tibiletti)

## Scarica l'ultima versione

<!-- APP_VERSION_BLOCK_START -->
**Versione disponibile: v0.3.9.1** — il numero è riportato anche sui pulsanti. I pulsanti scaricano l'ultima build completata per ciascun sistema operativo.

[![Windows 64 bit — scarica v0.3.9.1](https://img.shields.io/badge/Windows%2064%20bit-Scarica%20v0.3.9.1-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.9.1/VDV_LIGHT.PRO.-.Windows.zip) [![Download Windows](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.9.1/VDV_LIGHT.PRO.-.Windows.zip?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.9.1)

[![macOS Apple Silicon — M1, M2, M3, M4 — v0.3.9.1](https://img.shields.io/badge/macOS-M1%20%2F%20M2%20%2F%20M3%20%2F%20M4%20v0.3.9.1-111111?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.9.1/VDV_LIGHT.PRO-arm64.dmg) [![Download macOS Apple Silicon](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.9.1/VDV_LIGHT.PRO-arm64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.9.1)

[![macOS Intel — v0.3.9.1](https://img.shields.io/badge/macOS-Intel%20v0.3.9.1-555555?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.9.1/VDV_LIGHT.PRO-x86_64.dmg) [![Download macOS Intel](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.9.1/VDV_LIGHT.PRO-x86_64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.9.1)
<!-- APP_VERSION_BLOCK_END -->

[Altri download e versioni precedenti](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases)

## Installazione

### Windows

1. Scarica **VDV_LIGHT PRO — Windows.zip**.
2. Estrai tutto il contenuto in una cartella.
3. Avvia `VDV_LIGHT PRO.exe` dalla cartella estratta.

L'installer include ffmpeg e ffprobe per la riproduzione video.

### macOS

1. Scarica il DMG adatto al Mac: **Apple Silicon** per M1/M2/M3/M4 oppure **Intel** per i Mac Intel.
2. Apri il DMG e trascina **VDV_LIGHT PRO.app** in **Applicazioni**.
3. Espelli il DMG e avvia l'app. Se macOS mostra un avviso, fai clic destro sull'app in Applicazioni e scegli **Apri**.

Per riprodurre video su Mac serve ffmpeg, installabile con brew install ffmpeg. Audio, immagini, testi e luci funzionano senza ffmpeg.

## Cosa puoi fare

- Preparare e mandare cue con GO, barra spaziatrice, pause, attese, dissolvenze, gruppi e seguito automatico.
- Riprodurre audio, video, immagini e testi su uno schermo di uscita.
- Controllare luci DMX via Art-Net, sACN o interfaccia ENTTEC USB Pro.
- Creare e gestire patch e librerie di fari.
- Importare da QLab 5 cue, fari, indirizzi DMX e livelli.

Per segnalare un problema o proporre un miglioramento, apri una [segnalazione](https://github.com/teotibi/VDV-LIGHT-PRO/issues).
