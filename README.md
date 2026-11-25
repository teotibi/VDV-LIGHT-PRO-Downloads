# VDV_LIGHT PRO

**Regia per spettacoli teatrali su macOS e Windows.** Gestisce cue, audio, video, immagini, testi e luci DMX da un'unica interfaccia. Importa i progetti QLab 5.

<!-- CHANGELOG_START -->
## Cosa c'è di nuovo in v0.4.0

VDV_LIGHT PRO — novità della versione 0.4.0
Autore: Matteo Tibiletti

Pagina download — versione 0.4.0
Questa versione aggiunge il menu «Salva…» nella dashboard luci (nel cue
corrente, in un cue nuovo o negli appunti) con l'incolla delle impostazioni su
uno o più cue, la chiusura delle finestre con Ctrl/Cmd+W senza chiudere il
progetto per sbaglio, la dissolvenza automatica del secondo Esc e il cue BUIO
già pronto, sul tasto B, in ogni nuovo workspace. Gli show salvati con le
versioni 0.3.x si aprono senza problemi: al primo avvio le impostazioni vengono
solo aggiornate al nuovo numero di versione.

Novità rispetto alla 0.3.9.3

Dashboard luci: pulsante «Salva…»
- In basso a destra c'è un pulsante combinato «💾 Salva…» con tre voci:
  «Salva nel cue corrente» (chiede «Stai sovrascrivendo il contenuto del cue
  attualmente selezionato, sei sicuro?» con Sì e No), «Salva le impostazioni in
  un nuovo cue luci» e «Copia le impostazioni negli appunti».
- Per «impostazioni» si intendono tutti i fari come sono adesso. I canali DMX
  vengono salvati come valori interi, come fa QLab quando fotografa le luci.
- «Copia le impostazioni negli appunti» mette negli appunti un testo leggibile
  (un faro per riga, solo i canali non a riposo) e tiene le impostazioni anche
  dentro il programma.
- Tasto destro su un cue › «Incolla impostazioni nel cue selezionato»: incolla
  le impostazioni copiate nel cue, oppure in tutti i cue luci selezionati insieme
  («…nei cue selezionati (N)»); un solo passo di annulla. Disattivato finché non
  hai copiato qualcosa. Scorciatoia predefinita Cmd+Alt+V (modificabile).

Chiusura delle finestre con Ctrl/Cmd+W
- Se in primo piano c'è una finestra (dashboard, impostazioni luci DMX,
  movimento, mixer, calibrazione, impostazioni, novità, info, guida…) la
  scorciatoia chiude solo quella. Se in primo piano c'è la finestra del
  progetto, chiude il progetto con la richiesta di salvare le modifiche.
- Le finestre separate (timeline, keypad, monitor DMX, schermo di uscita) si
  chiudono da sole quando sono quelle attive. Con una domanda aperta la
  scorciatoia non fa nulla.

Esc
- Il primo Esc sfuma tutto come prima. Il secondo Esc, mentre la dissolvenza è in
  corso, ora applica a audio, video e immagini in esecuzione una dissolvenza di
  chiusura automatica di 2 secondi (invece di fermarli di colpo); gli altri cue si
  fermano subito. La durata si cambia in Impostazioni › Generale («Dissolvenza
  del secondo Esc», 0 = si fermano subito). Un terzo Esc ferma tutto subito.

Nuovi workspace
- Ogni nuovo workspace (schermata iniziale, «Nuovo show», dopo la chiusura
  dell'ultimo file) parte con il cue BUIO già in lista, con il trigger sul tasto
  B. Se avevi tolto il BUIO dal menu Preset il workspace resta vuoto. I file che
  apri o importi non vengono modificati.

Regole verificate su QLab (indirizzi delle funzioni in MECHANICS.md)
- Istantanea delle luci (valori arrotondati alla precisione di visualizzazione),
  incolla attivo solo dopo una copia, domanda di chiusura con tre risposte,
  secondo panic di QLab (ferma subito: qui è sostituito dalla dissolvenza).

Versione
- La versione passa a 0.4.0: il numero interno («build») diventa 400, quindi le
  vecchie impostazioni vengono aggiornate una volta, senza toccare show e
  libreria fari.

Cosa non c'è (ancora)
- Il filtro di QLab che lascia fuori dall'istantanea i valori a riposo non è
  stato capito: qui vengono salvati tutti i canali.
- Il comando di chiusura con Ctrl/Cmd+W non chiude da solo le finestre di
  dialogo (ad esempio «Nuovo gruppo»): vanno chiuse con i loro pulsanti.

<!-- CHANGELOG_END -->

## Ricevi gli aggiornamenti via email

Iscriviti per ricevere un messaggio quando viene pubblicata una nuova versione, con il numero della release, l’elenco delle novità e il link diretto alla pagina ufficiale dei download. Puoi annullare l’iscrizione in qualsiasi momento dal link presente in ogni email.

[Iscriviti agli aggiornamenti di VDV_LIGHT PRO](https://buttondown.com/tibiletti)

## Scarica l'ultima versione

<!-- APP_VERSION_BLOCK_START -->
**Versione disponibile: v0.4.0** — il numero è riportato anche sui pulsanti. I pulsanti scaricano l'ultima build completata per ciascun sistema operativo.

[![Windows 64 bit — scarica v0.4.0](https://img.shields.io/badge/Windows%2064%20bit-Scarica%20v0.4.0-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.0/VDV_LIGHT.PRO.-.Windows.zip) [![Download Windows](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.0/VDV_LIGHT.PRO.-.Windows.zip?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.0)

[![macOS Apple Silicon — M1, M2, M3, M4 — v0.4.0](https://img.shields.io/badge/macOS-M1%20%2F%20M2%20%2F%20M3%20%2F%20M4%20v0.4.0-111111?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.0/VDV_LIGHT.PRO-arm64.dmg) [![Download macOS Apple Silicon](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.0/VDV_LIGHT.PRO-arm64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.0)

[![macOS Intel — v0.4.0](https://img.shields.io/badge/macOS-Intel%20v0.4.0-555555?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.0/VDV_LIGHT.PRO-x86_64.dmg) [![Download macOS Intel](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.0/VDV_LIGHT.PRO-x86_64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.0)
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
