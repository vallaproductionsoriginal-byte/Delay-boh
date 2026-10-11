# Delay-boh

Plug-in delay gratuito di **Valla Productions** per **macOS Apple Silicon**, versione **1.0.1**, nei formati **VST3 e Audio Unit (AU)**.

[Scarica Delay-boh 1.0.1](https://github.com/vallaproductionsoriginal-byte/Delay-boh/releases/download/v1.0.1/Delay-boh-1.0.1-mac-arm64.zip) · [Tutte le release](https://github.com/vallaproductionsoriginal-byte/Delay-boh/releases)

![Interfaccia di Delay-boh: controlli del delay e pagina Time / Sync](docs/Delay-boh-interface.png)

## Requisiti

- Mac Apple Silicon, architettura arm64.
- macOS 11 o successivo.
- DAW o host compatibile con plug-in VST3 o Audio Unit arm64.

## Installazione

1. Scarica e apri lo ZIP della release.
2. Installa il formato usato dalla tua DAW: copia `Delay-boh.vst3` in `~/Library/Audio/Plug-Ins/VST3/` oppure `Delay-boh.component` in `~/Library/Audio/Plug-Ins/Components/`. Puoi installare entrambi. Crea le cartelle se mancano; nel Finder puoi aprire ciascun percorso con **Vai → Vai alla cartella…**.
3. Riavvia la DAW o avvia una nuova scansione dei plug-in.
4. Carica **Delay-boh** tra gli effetti di **Valla Productions**. Il formato AU per macOS è il bundle `.component`.

Lo ZIP include entrambi i formati. Conserva `LICENSE`, `THIRD_PARTY_NOTICES.md` e la cartella `licenses` se redistribuisci il pacchetto. Una copia delle licenze è inclusa anche nei bundle.

I bundle hanno una firma ad hoc e non sono notarizzati da Apple. macOS potrebbe richiedere un'autorizzazione di sicurezza: dopo un eventuale blocco, controlla **Impostazioni di Sistema → Privacy e sicurezza** e autorizza il plug-in solo se proviene da questa release.

## Funzioni

- 17 modalità: Tape, HiFi, BBD, Digital, Ghost, Pitch, RevPitch, DuckTape, Clarity, BBDuck, LoFi, Analog, ChromeTape, Quartz, PhaserDDL, PitchDuck e RichPitch.
- 5 stili: Single, Dual, Ratio, PingPong e Quad; tempi da 1 ms a 10 secondi.
- Sync al BPM dell'host, note regolari, puntate e terzinate.
- Quattro tap, feedback positivo o negativo, Repeat/Swell e ducking.
- Drive, age, era, width, filtri low/high cut e diffusione.
- Wow/flutter, frequency shift, pitch shift, reverse e phaser.
- 38 parametri automatizzabili, nove preset di partenza e Mix Lock.
- Ingresso e uscita stereo o mono.

Per impostare il tempo destro in modo indipendente, usa Dual, PingPong o Quad. Le pagine Time/Sync, Tone/Space, Mod/Pitch e Quad/Feedback raggruppano gli altri controlli. Doppio clic su un controllo continuo per ripristinarne il valore iniziale.

## Verifica della release

La release include un file con il checksum SHA-256 tra gli allegati. Dopo aver scaricato lo ZIP e il file `.sha256` nella stessa cartella, puoi verificarlo con:

```sh
shasum -a 256 -c Delay-boh-1.0.1-mac-arm64.zip.sha256
```

Build arm64 e firme dei bundle verificate, test DSP e host VST3/AU superati, Audio Unit validato con `auval`. La versione è stata verificata su un Mac Apple Silicon; non sono dichiarati test su tutte le versioni di macOS o su tutte le DAW.

## Licenza

Delay-boh e la documentazione del progetto sono distribuiti sotto [licenza MIT](LICENSE). Questa release distribuisce il plug-in compilato; i sorgenti non sono inclusi.

Le componenti di terze parti mantengono le proprie licenze e non sono rilicenziate sotto la MIT del progetto. JUCE 9.0.3 è utilizzato dal distributore sotto licenza commerciale **JUCE Starter**. Le attribuzioni e i testi delle licenze sono in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) e nella cartella [licenses](licenses).

## Problemi e feedback

Segnala problemi tramite le [Issues](https://github.com/vallaproductionsoriginal-byte/Delay-boh/issues), indicando versione di macOS, modello di Mac, DAW e passaggi per riprodurli.
