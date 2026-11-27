# VDV_LIGHT PRO

**Regia per spettacoli teatrali su macOS e Windows.** Gestisce cue, audio, video, immagini, testi e luci DMX da un'unica interfaccia. Importa i progetti QLab 5.

<!-- CHANGELOG_START -->
## Cosa c'è di nuovo in v0.4.2

VDV_LIGHT PRO — novità della versione 0.4.2
Autore: Matteo Tibiletti

Pagina download — versione 0.4.2
Questa versione porta il PALCO a un impianto completo: preset impianto luci a portata di mano e salvabili su file (da tenere su Drive), casse audio sul palco con il bilanciamento di ogni suono, e tre comodità sulla lista dei cue: «Copia / Incolla attributi», Cmd+A per selezionare tutto e la domanda «Dissolvenza» con più cue scelti. Gli show e le impostazioni delle versioni 0.4.x si aprono senza problemi.

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
**Versione disponibile: v0.4.2** — il numero è riportato anche sui pulsanti. I pulsanti scaricano l'ultima build completata per ciascun sistema operativo.

[![Windows 64 bit — scarica v0.4.2](https://img.shields.io/badge/Windows%2064%20bit-Scarica%20v0.4.2-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.2/VDV_LIGHT.PRO.-.Windows.zip) [![Download Windows](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.2/VDV_LIGHT.PRO.-.Windows.zip?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.2)

[![macOS Apple Silicon — M1, M2, M3, M4 — v0.4.2](https://img.shields.io/badge/macOS-M1%20%2F%20M2%20%2F%20M3%20%2F%20M4%20v0.4.2-111111?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.2/VDV_LIGHT.PRO-arm64.dmg) [![Download macOS Apple Silicon](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.2/VDV_LIGHT.PRO-arm64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.2)

[![macOS Intel — v0.4.2](https://img.shields.io/badge/macOS-Intel%20v0.4.2-555555?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/download/v0.4.2/VDV_LIGHT.PRO-x86_64.dmg) [![Download macOS Intel](https://img.shields.io/github/downloads/teotibi/VDV-LIGHT-PRO-Downloads/v0.4.2/VDV_LIGHT.PRO-x86_64.dmg?label=download&style=flat-square)](https://github.com/teotibi/VDV-LIGHT-PRO-Downloads/releases/tag/v0.4.2)
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
