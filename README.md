# VDV_LIGHT PRO

**Regia per spettacoli teatrali su macOS e Windows.** Gestisce cue, audio, video, immagini, testi e luci DMX da un'unica interfaccia. Importa i progetti QLab 5.

<!-- CHANGELOG_START -->
## Cosa c'è di nuovo in v0.3.9.3

VDV_LIGHT PRO — novità della versione 0.3.9.3
Autore: Matteo Tibiletti

Pagina download — versione 0.3.9.3
Questa versione aggiunge il Monitor DMX in tempo reale (che sostituisce la
vista dei fari accesi nel pannello di destra), il menu «Finestre» e la modifica
dei valori dal monitor con cursori, ANNULLA e SALVA. Gli show salvati con la
0.3.9.2 e le versioni precedenti si aprono senza problemi.

Novità rispetto alla 0.3.9.2

Monitor DMX (pannello di destra)
- Il pannello di destra si apre sul nuovo «Monitor DMX», ispirato al Banco
  Semplice di QLC+: un menu Universo e una colonna per ogni canale DMX, affiancate
  e con scorrimento orizzontale. Ogni colonna mostra una barra verticale, il
  valore reale 0–255 e il numero del canale, con il nome della funzione (Pan,
  Tilt, Intensità…) in alto quando il faro è noto. Passando il mouse si vede il
  faro e il canale.
- Mostra quello che il programma sta davvero mandando in uscita (dopo Blackout e
  dopo il keyframe in modifica), non il valore impostato nell'interfaccia, così
  si vede se un canale, per esempio un movimento, cambia perché lo hai comandato
  tu o da solo. Si aggiorna circa 30 volte al secondo.
- Un canale che cambia lampeggia in giallo e poi si calma; i canali a zero sono in
  tono spento. Filtri: «solo canali dei fari» e «solo valori ≠ 0».
- Vista «griglia 16×32»: tutti i 512 canali insieme in una griglia di 16 colonne
  per 32 righe, come la finestra DMX di QLab (un valore in ogni cella, lampeggio
  quando cambia, il faro e il canale passando il mouse). La vista a colonne resta
  quella predefinita e l'unica modificabile.
- Se nessuna uscita DMX è attiva, lo dice: i valori sono quelli che verrebbero
  inviati. La vista dei fari accesi resta nella scheda «Luci».

Monitor in finestra separata
- «⧉ Stacca» apre il monitor in una finestra a parte, che si può spostare e
  ridimensionare (le barre seguono l'altezza); «⮌ Aggancia» (o chiudere la
  finestra) lo riporta a destra. Lo stesso comando è nel menu Finestre.

Modifica dal monitor
- Con la riproduzione ferma (Esc) il pulsante «✏ Modifica» si attiva: le barre
  diventano cursori con una stanghetta orizzontale ben visibile, da trascinare o
  cliccare. Sotto ogni cursore il valore (in DMX oppure in %, a scelta) cambia in
  diretta e si può anche scrivere a mano.
- Le luci seguono subito. «ANNULLA» rimette tutto com'era prima della modifica;
  «SALVA» tiene i valori come quelli impostati nella dashboard (e li scrive nel
  cue che stai modificando lì). Se parte una riproduzione durante la modifica,
  la modifica viene annullata.
- Per Pan e Tilt il valore tiene conto della calibrazione della testa. I canali
  a 16 bit, quelli senza faro e quelli spenti non si modificano.

Menu «Finestre»
- Nuovo menu in alto che raggruppa tutte le finestre: Dashboard luci, Movimento
  (apre quello selezionato o ne crea uno), Impostazioni luci DMX, Monitor DMX
  (anche in finestra separata), Schermo, Schermo di uscita, Palco 3D, Timeline
  separata, Mixer, Keypad, Impostazioni, più un sottomenu «Aggiungi» con tutti i
  comandi della barra (tipi di cue, Movimento, Preset, Keypad).

Regole verificate su QLab (indirizzi delle funzioni in MECHANICS.md)
- Finestra «DMX status» di QLab: 512 canali per universo in una griglia 16×32,
  256 livelli di valore, aggiornamento al massimo ogni 0,1 s (il monitor è più
  veloce di proposito), valore scritto tagliato tra 0 e 255, una sola finestra
  riutilizzata.

Cosa non c'è (ancora)
- Nel monitor di QLab i valori scritti vanno subito alle luci; qui sono una
  bozza con ANNULLA e SALVA, e solo a riproduzione ferma (scelta voluta).
- Le note di scena (teste mobili grandi che non arrivano al pianoforte, teste
  piccole sfocate, controluce rosso per Sara) non sono modifiche al programma e
  non sono incluse; il preset «Sara – controluce rosso» non è stato creato.
<!-- CHANGELOG_END -->

## Ricevi gli aggiornamenti via email

Iscriviti per ricevere un messaggio quando viene pubblicata una nuova versione, con il numero della release, l’elenco delle novità e il link diretto alla pagina ufficiale dei download. Puoi annullare l’iscrizione in qualsiasi momento dal link presente in ogni email.

[Iscriviti agli aggiornamenti di VDV_LIGHT PRO](https://buttondown.com/tibiletti)

## Scarica l'ultima versione

<!-- APP_VERSION_BLOCK_START -->
**Versione disponibile: v0.3.9.3** — il numero è riportato anche sui pulsanti. I pulsanti scaricano l'ultima build completata per ciascun sistema operativo.

[![Windows 64 bit — scarica v0.3.9.3](https://img.shields.io/badge/Windows%2064%20bit-Scarica%20v0.3.9.3-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.9.3/VDV_LIGHT.PRO.-.Windows.zip) [![Download Windows](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.9.3/VDV_LIGHT.PRO.-.Windows.zip?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.9.3)

[![macOS Apple Silicon — M1, M2, M3, M4 — v0.3.9.3](https://img.shields.io/badge/macOS-M1%20%2F%20M2%20%2F%20M3%20%2F%20M4%20v0.3.9.3-111111?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.9.3/VDV_LIGHT.PRO-arm64.dmg) [![Download macOS Apple Silicon](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.9.3/VDV_LIGHT.PRO-arm64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.9.3)

[![macOS Intel — v0.3.9.3](https://img.shields.io/badge/macOS-Intel%20v0.3.9.3-555555?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.9.3/VDV_LIGHT.PRO-x86_64.dmg) [![Download macOS Intel](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.9.3/VDV_LIGHT.PRO-x86_64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.9.3)
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
