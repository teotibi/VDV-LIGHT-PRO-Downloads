# VDV_LIGHT PRO

**Regia per spettacoli teatrali su macOS e Windows.** Gestisce cue, audio, video, immagini, testi e luci DMX da un'unica interfaccia. Importa i progetti QLab 5.

<!-- CHANGELOG_START -->
## Cosa c'è di nuovo in v0.4.3.1

VDV_LIGHT PRO — novità della versione 0.4.3.1
Autore: Matteo Tibiletti

Pagina download — versione 0.4.3.1
La 0.4.3.1 arriva subito dopo la 0.4.3, quindi qui trovi le novità di tutte e due. Nella lista dei cue ora puoi allargare le colonne a mano o farle adattare al contenuto, così i titoli lunghi si leggono per intero. Gli show e le impostazioni delle versioni 0.4.x si aprono senza problemi.

Novità della 0.4.3.1

Lista dei cue: colonne regolabili
- Trascina il divisorio tra due colonne dell'intestazione per allargare quella a sinistra (quella a destra si restringe).
- Doppio clic sul divisorio: la colonna si adatta al testo più lungo che contiene (titoli dei brani, nomi dei file e destinazioni).
- Clic destro sull'intestazione: le colonne tornano come all'inizio.
- Larghezze minime: «N°» e «Poi» 30, «Attesa prima» e «Durata» 60 (come nell'originale). Le larghezze non si salvano ancora alla chiusura del programma.
- La lista dei cue è quella di sempre: la ricostruzione da zero fatta per errore è stata scartata.

Novità della 0.4.3 (rielencate qui)

Monitor DMX
- Una colonna per ogni canale DMX con barra, valore reale 0–255 e numero del canale: mostra quello che il programma sta davvero inviando, anche durante blackout e modifica dei keyframe. Un canale che cambia lampeggia.
- In sola lettura finché la riproduzione è in corso; con Esc e «Modifica» le barre diventano cursori da trascinare o scrivere (DMX o %), con ANNULLA e SALVA. Può stare in una finestra a parte (Stacca / Aggancia).

Finestre e comandi
- Cmd+W (Ctrl+W) chiude la finestra in primo piano e chiude il progetto solo se è lui la finestra davanti.
- Tasto destro su un cue luci: «Incolla impostazioni» copia nel cue (o in tutti quelli selezionati) le impostazioni copiate dalla dashboard.

Interfacce DMX USB
- Riconoscimento delle interfacce ENTTEC DMX USB Pro (nome, firmware) e ricerca dei fari RDM dietro di esse.

Novità della 0.4.2

Lista dei cue
- Cmd+A (Ctrl+A) seleziona tutti i cue; Canc o Backspace li elimina tutti insieme (un solo Cmd+Z li riporta indietro). C'è anche Modifica › «Seleziona tutti i cue».
- «Dissolvenza» con due o più cue scelti (audio, video, immagini, luci) apre la domanda: aggiungi una dissolvenza per ogni cue dopo l'ultimo selezionato; inserisci una dissolvenza dopo ogni cue; aggiungi una sola dissolvenza senza destinazione. I tasti 1, 2, 3 funzionano come scorciatoie e la scelta fatta per ultima resta evidenziata la volta dopo.

Copia e incolla attributi (tasto destro su un cue)
- «Copia attributi» (Cmd+Ctrl+C) copia tutto quello che è impostato in un cue: volume, dissolvenze, attese, luci, uscita audio…
- «Incolla attributi…» (Cmd+Ctrl+V), su un cue dello stesso tipo (audio con audio, video con video, luci con luci), apre una finestra con una spunta per ogni attributo, con accanto il valore copiato: puoi incollare tutto o solo alcune cose (solo il volume, solo la dissolvenza, solo i fari scelti con i loro valori…). Il pulsante «Ultimi usati» spunta gli attributi incollati l'ultima volta. Su più cue insieme in un solo passo di annulla. Su Windows e Linux le scorciatoie sono Ctrl+Maiusc+C e Ctrl+Maiusc+V.

PALCO: preset impianto luci
- Nella barra del PALCO c'è il pulsante «⭐ Preset» (lo stesso menu di «Aggiungi › Preset») e, nella colonna a sinistra, i preset impianto in memoria: un clic e l'impianto torna, con i fari, i nomi, gli indirizzi e le posizioni sul palco 3D (Cmd+Z per tornare indietro).
- Nel menu Preset: «Salva gli impianti in un file…» e «Carica impianti da un file…» (il formato è JSON), il pulsante 💾 su ogni preset per salvare solo quello, e lo stesso per i preset di cue. Caricando un file con un solo impianto, l'impianto viene richiamato subito nel workspace; con più impianti vanno in memoria e se ne richiama uno dal menu. Un preset con lo stesso nome viene sostituito: così un backup su Drive ripristina tutto.
- Anche le casse audio e la modalità audio dello show viaggiano con il preset e con il file. I preset salvati con le versioni precedenti non hanno le casse: richiamali, sistema le casse e aggiornali con ↻.

PALCO: casse audio e bilanciamento
- Nel pannello a destra, «Casse audio»: aggiungi, dai un nome e posiziona le casse (anche trascinandole sul palco in EDIT); si disegnano nella vista 3D e si salvano con lo show. Lì c'è anche «Audio dello show»: stereo, mono o surround.
- Su ogni cue audio, Dettagli › Audio › «Uscita audio»: modalità propria (o come lo show) e le casse a cui mandare il suono: tutte, solo sinistra, solo destra o un livello per ciascuna. Il surround riduce a stereo i file 5.1 e 7.1.
- Il programma suona su un'unica uscita stereo: ogni cassa diventa un bilanciamento sinistra/destra in base a dove la metti sul palco. L'uscita separata per ogni cassa (scheda audio multicanale) non c'è ancora.

Versione
- La versione passa a 0.4.2 (numero interno 402): le impostazioni salvate dalla 0.4.1 vengono solo aggiornate al nuovo numero, show e libreria fari non si toccano.

<!-- CHANGELOG_END -->

## Ricevi gli aggiornamenti via email

Iscriviti per ricevere un messaggio quando viene pubblicata una nuova versione, con il numero della release, l’elenco delle novità e il link diretto alla pagina ufficiale dei download. Puoi annullare l’iscrizione in qualsiasi momento dal link presente in ogni email.

[Iscriviti agli aggiornamenti di VDV_LIGHT PRO](https://buttondown.com/tibiletti)

## Scarica l'ultima versione

<!-- APP_VERSION_BLOCK_START -->
**Versione disponibile: v0.4.3.1** — il numero è riportato anche sui pulsanti. I pulsanti scaricano l'ultima build completata per ciascun sistema operativo.

[![Windows 64 bit — scarica v0.4.3.1](https://img.shields.io/badge/Windows%2064%20bit-Scarica%20v0.4.3.1-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.3.1/VDV_LIGHT.PRO.-.Windows.zip) [![Download Windows](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.3.1/VDV_LIGHT.PRO.-.Windows.zip?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.3.1)

[![macOS Apple Silicon — M1, M2, M3, M4 — v0.4.3.1](https://img.shields.io/badge/macOS-M1%20%2F%20M2%20%2F%20M3%20%2F%20M4%20v0.4.3.1-111111?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.3.1/VDV_LIGHT.PRO-arm64.dmg) [![Download macOS Apple Silicon](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.3.1/VDV_LIGHT.PRO-arm64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.3.1)

[![macOS Intel — v0.4.3.1](https://img.shields.io/badge/macOS-Intel%20v0.4.3.1-555555?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.3.1/VDV_LIGHT.PRO-x86_64.dmg) [![Download macOS Intel](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.3.1/VDV_LIGHT.PRO-x86_64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.3.1)
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
