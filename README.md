# YQArch Italiano

Localizzazione e modernizzazione italiana gratuita di **YQArch per AutoCAD**.

**Versione corrente: 3.78**

Verifiche automatiche della 3.78 e CUIx identico alla **3.77 collaudata su AutoCAD 2027 italiano**: 646/646 comandi definiti, zero mancanti, menu e altezza Ribbon confermati. Il report nativo non esegue i comandi né certifica ogni risultato geometrico. Le altre combinazioni AutoCAD/Windows restano da verificare su installazioni reali.

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
| Primaria | AutoCAD 2021–2027 | collaudo nativo 3.77 su AutoCAD 2027 italiano; stesso CUIx nella 3.78; altre versioni da verificare |
| Estesa | AutoCAD 2015–2020 | controlli statici; collaudo reale richiesto sulla specifica versione |
| Legacy | AutoCAD 2007–2014 | best effort |
| Legacy parziale | AutoCAD 2004–2006 | 147/195 DWG del catalogo sono in formati leggibili; 48 blocchi AC1021 richiedono AutoCAD 2007+ e vengono intercettati prima dell'inserimento |

L'installer `YQArch_Italiano_3.78.exe` è destinato a **Windows x64** nelle combinazioni supportate dalla specifica versione di AutoCAD. Per installazioni legacy è disponibile il pacchetto ZIP con procedura manuale.

> La compatibilità di YQArch Italiano non rende supportata una combinazione AutoCAD/Windows che Autodesk non supporta ufficialmente. Verifica sempre i requisiti Autodesk della release di AutoCAD utilizzata.

## Installazione

1. Chiudere AutoCAD.
2. Scaricare l'installer verificato dalla pagina **YQArch Italiano** su [andreagiaquinto.it/yqarch-italiano/](https://andreagiaquinto.it/yqarch-italiano/).
3. Avviare `YQArch_Italiano_3.78.exe`.
4. Riaprire AutoCAD.
5. Eseguire `YQIT_DIAGNOSTICA_COMPLETA`.

L’EXE non è firmato Authenticode: Windows SmartScreen può mostrare un avviso di reputazione. Controllare provenienza e SHA-256 senza disattivare le protezioni di Windows.

La Ribbon conserva 10 pannelli: un grande affiancato a cinque piccoli (3+2), più sette accessi nel flyout per pannello. Sono 60 accessi visibili e 70 nel flyout, 130 in totale; 23 categorie e 547 voci storiche conservate. Nel catalogo: **Seleziona → Inserisci → clic nel DWG → inserimento completato**. Il comportamento del catalogo è conservato; la verifica delle definizioni non equivale al collaudo individuale dei 646 comandi.

Per installazioni legacy utilizzare il pacchetto ZIP e consultare `INSTALLAZIONE_LEGACY.md`.

## Verifica installazione

In AutoCAD sono disponibili:

- `YQIT_DIAGNOSTICA_COMPLETA` — verifica il caricamento del runtime e il registro dei 646 comandi;
- `YQIT_COMPATIBILITA` — mostra versione AutoCAD, piattaforma, LISPSYS e fascia di compatibilità.

## Integrità versione 3.78

- EXE SHA-256: `f134c2783721956daea5d3c1176302f31c944bcdc68f332ae87894b2a36c8cc9`
- ZIP SHA-256: `ecd56dd0238cd9a949a452a922e2b67075d2d09c9ac04cd5851f88ed79e48c4b`

## Documentazione

Nel repository sono disponibili le note di rilascio, la matrice di compatibilità e le istruzioni di installazione legacy. La guida completa e i download verificati sono pubblicati anche nella pagina YQArch Italiano del sito.

## Progetto originale

YQArch Italiano è una localizzazione e modernizzazione indipendente del progetto YQArch originale. Il progetto originale, i relativi autori e le relative risorse mantengono la propria identità e attribuzione.
