# YQArch Italiano

Localizzazione e modernizzazione italiana gratuita di **YQArch per AutoCAD**.

**Versione corrente: 3.73**  
Collaudo reale della release 3.73: **AutoCAD 2026 italiano** nell’ambiente dell’autore. Le altre combinazioni AutoCAD/Windows restano da verificare su installazioni reali.

## Stato del progetto

- registro verificato di **646 comandi**;
- guida italiana con **646 schede**;
- prompt, menu, finestre e pannelli sottoposti a revisione massiva;
- diagnostica integrata con `YQIT_DIAGNOSTICA_COMPLETA` e `YQIT_COMPATIBILITA`;
- core storico conservato quando stabile;
- `SECURELOAD` e `TRUSTEDPATHS` non vengono modificati.

## Compatibilità

| Fascia | Versioni AutoCAD per Windows | Stato |
|---|---|---|
| Primaria | AutoCAD 2021–2027 | collaudo reale su AutoCAD 2026 italiano; altre versioni della fascia da verificare su installazioni reali |
| Estesa | AutoCAD 2015–2020 | controlli statici; collaudo reale richiesto sulla specifica versione |
| Legacy | AutoCAD 2007–2014 | best effort |
| Legacy parziale | AutoCAD 2004–2006 | 147/195 DWG del catalogo sono in formati leggibili; 48 blocchi AC1021 richiedono AutoCAD 2007+ e vengono intercettati prima dell'inserimento |

L'installer `YQArch_Italiano_3.73.exe` è destinato a **Windows x64** nelle combinazioni supportate dalla specifica versione di AutoCAD. Per installazioni legacy è disponibile il pacchetto ZIP con procedura manuale.

> La compatibilità di YQArch Italiano non rende supportata una combinazione AutoCAD/Windows che Autodesk non supporta ufficialmente. Verifica sempre i requisiti Autodesk della release di AutoCAD utilizzata.

## Installazione

1. Chiudere AutoCAD.
2. Scaricare l'installer verificato dalla pagina **YQArch Italiano** su [andreagiaquinto.it/yqarch-italiano/](https://andreagiaquinto.it/yqarch-italiano/).
3. Avviare `YQArch_Italiano_3.73.exe`.
4. Riaprire AutoCAD.
5. Eseguire `YQIT_DIAGNOSTICA_COMPLETA`.

L’EXE non è firmato Authenticode: Windows SmartScreen può mostrare un avviso di reputazione. Controllare provenienza e SHA-256 senza disattivare le protezioni di Windows.

La Ribbon conserva 10 pannelli, ciascuno con 3 icone grandi e 10 piccole: 130 accessi diretti. Nel catalogo: **Seleziona → Inserisci → clic nel DWG → inserimento completato**. Questo flusso è stato collaudato nell’ambiente indicato; non equivale al collaudo individuale dei 646 comandi.

Per installazioni legacy utilizzare il pacchetto ZIP e consultare `INSTALLAZIONE_LEGACY.md`.

## Verifica installazione

In AutoCAD sono disponibili:

- `YQIT_DIAGNOSTICA_COMPLETA` — verifica il caricamento del runtime e il registro dei 646 comandi;
- `YQIT_COMPATIBILITA` — mostra versione AutoCAD, piattaforma, LISPSYS e fascia di compatibilità.

## Integrità versione 3.73

- EXE SHA-256: `07165f6a941ebb4b97e4842d4cdf4a03a017bd433cda8a17eb8f7aa419c6280d`
- ZIP SHA-256: `ec14d087067620222a721da25c1034167edb9411741ac5fe5dc69ba76c839df2`

## Documentazione

Nel repository sono disponibili le note di rilascio, la matrice di compatibilità e le istruzioni di installazione legacy. La guida completa e i download verificati sono pubblicati anche nella pagina YQArch Italiano del sito.

## Progetto originale

YQArch Italiano è una localizzazione e modernizzazione indipendente del progetto YQArch originale. Il progetto originale, i relativi autori e le relative risorse mantengono la propria identità e attribuzione.
