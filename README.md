# VDV_LIGHT PRO

**Regia per spettacoli teatrali su macOS e Windows.** Gestisce cue, audio, video, immagini, testi e luci DMX da un'unica interfaccia. Importa i progetti QLab 5.

<!-- CHANGELOG_START -->
## Cosa c'è di nuovo in v0.3.7

**VDV_LIGHT PRO — novità della versione 0.3.7**  
Autore: Matteo Tibiletti

**Tutti i cambiamenti di questa giornata:**

**Calibrazione delle teste mobili**
- L'anteprima 3D del palco, nella finestra «Calibra», ora è collegata alla testa mobile: la luce si accende e il fascio si muove mentre sposti Pan e Tilt (prima la testa disegnata restava ferma e spenta).
- L'anteprima mostra la stessa cosa che va al faro vero: dimmer e colore al massimo, tutti gli altri canali (Pan, Tilt, zoom…) dai valori che stai impostando.
- La calibrazione parte dalla posizione già salvata (o dal centro) invece che da Pan 0 / Tilt 0, così il fascio punta subito il palco e si vede.
- La posizione che salvi con «Salva calibrazione» diventa lo «0» della testa e viene salvata anche nei preset dell'impianto luci, insieme ai fari. Il testo della finestra lo spiega e, dopo il salvataggio, compare un messaggio.
- Il quadratino Pan/Tilt si muove anche con lo scorrimento a due dita sul trackpad (il doppio più veloce) o con la rotella (metà velocità), con il verticale invertito, come in QLab.

**Scorciatoie da tastiera (Impostazioni › Scorciatoie da tastiera)**
- Nuovi comandi «Nuovo cue …» per ogni tipo di cue: Audio, Dissolvenza, Video, Luci, Attesa, Promemoria, Sequenza, Avvia cue, Ferma cue, Pausa cue, Vai a, Ferma tutto e Movimento.
- Già assegnate: Cmd+Maiusc+A (audio), +F (dissolvenza), +V (video), +L (luci), +W (attesa). Gli altri comandi sono liberi: li scegli tu con «Cambia».
- Il tasto compare nel suggerimento dei pulsanti «Aggiungi», e un tasto rapido fa esattamente la stessa cosa del pulsante.
- L'elenco delle scorciatoie è più alto e scorre fino in fondo.
- Tasto rapido (trigger) di un cue: «Cancella» lo toglie; Tab, Invio, frecce e le combinazioni con Cmd vengono rifiutate con un messaggio (come in QLab).

**Passare da una finestra all'altra**
- Cmd+< (il tasto «<» della tastiera italiana, due soli tasti) passa da una finestra all'altra: finestra principale → finestre aperte (Impostazioni DMX, Calibra, Dashboard…) → di nuovo la principale. La finestra scelta sale in primo piano e si illumina per un attimo con un bordo verde acceso. Con Maiusc si torna indietro.
- Se chiedi una finestra già aperta (menu, scorciatoie, pulsanti), ora viene portata in primo piano invece di non fare nulla.

**Regole verificate sul programma originale (QLab)**
- Dissolvenze audio con curva a coseno e volume limitato ai valori del programma originale (-60 dB come minimo).
- Durate: i valori non validi o negativi vengono rifiutati; i tempi digitati seguono il formato rigoroso di QLab.
- Il cue «Target» con file apre una scelta di un solo file, senza filtri, e cambia solo se confermi con OK.
- Trigger MIDI: canale (qualsiasi o uno), tipo di messaggio e dati devono coincidere; nota con velocità 0 = rilascio. I comandi dell'app si imparano premendo il pulsante del controller.
- Schermo di uscita: l'elenco si aggiorna solo quando colleghi o scolleghi un monitor; lo schermo salvato si ritrova per produttore/modello/seriale, poi per nome, poi per posizione.
- Un secondo GO ravvicinato viene ignorato.
- Tutte le regole, con gli indirizzi delle funzioni di QLab, sono in MECHANICS.md.

**Versione e pacchetti**
- La versione dell'app è mostrata nel menu File e in «Info».
- Nuova voce Aiuto › «Novità di questa versione»: apre una finestra con queste note, come il «changelog» di QLab.
- Nuovi pacchetti 0.3.7 per Mac (.dmg) e Windows (.zip), con queste note.
<!-- CHANGELOG_END -->

## Ricevi gli aggiornamenti via email

Iscriviti per ricevere un messaggio quando viene pubblicata una nuova versione, con il numero della release, l’elenco delle novità e il link diretto alla pagina ufficiale dei download. Puoi annullare l’iscrizione in qualsiasi momento dal link presente in ogni email.

[Iscriviti agli aggiornamenti di VDV_LIGHT PRO](https://buttondown.com/tibiletti)

## Scarica l'ultima versione

<!-- APP_VERSION_BLOCK_START -->
**Versione disponibile: v0.3.7** — il numero è riportato anche sui pulsanti. I pulsanti scaricano l'ultima build completata per ciascun sistema operativo.

[![Windows 64 bit — scarica v0.3.7](https://img.shields.io/badge/Windows%2064%20bit-Scarica%20v0.3.7-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.7/VDV_LIGHT.PRO.-.Windows.zip) [![Download Windows](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.7/VDV_LIGHT.PRO.-.Windows.zip?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.7)

[![macOS Apple Silicon — M1, M2, M3, M4 — v0.3.7](https://img.shields.io/badge/macOS-M1%20%2F%20M2%20%2F%20M3%20%2F%20M4%20v0.3.7-111111?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.7/VDV_LIGHT.PRO-arm64.dmg) [![Download macOS Apple Silicon](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.7/VDV_LIGHT.PRO-arm64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.7)

[![macOS Intel — v0.3.7](https://img.shields.io/badge/macOS-Intel%20v0.3.7-555555?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.3.7/VDV_LIGHT.PRO-x86_64.dmg) [![Download macOS Intel](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.3.7/VDV_LIGHT.PRO-x86_64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.3.7)
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
