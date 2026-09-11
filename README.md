# YQArch Italiano

Localizzazione e modernizzazione italiana gratuita di **YQArch per AutoCAD**.

**Versione corrente: 3.61**  
Ambiente di riferimento e collaudo: **AutoCAD 2027 italiano su Windows 11 x64**.

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
| Primaria | AutoCAD 2021–2027 | progettata e verificata come fascia principale |
| Estesa | AutoCAD 2015–2020 | compatibilità tecnica verificata; consigliato collaudo reale |
| Legacy | AutoCAD 2008–2014 | best effort |
| Legacy parziale | AutoCAD 2004–2007 | alcune funzioni possono dipendere da capacità introdotte successivamente |

L'installer `YQArch_Italiano_3.61.exe` è destinato a **Windows 10/11 x64**. Per sistemi precedenti o installazioni a 32 bit è disponibile il pacchetto ZIP portabile con procedura manuale.

> La compatibilità di YQArch Italiano non rende supportata una combinazione AutoCAD/Windows che Autodesk non supporta ufficialmente. AutoCAD 2027, per esempio, richiede ufficialmente Windows 11 a 64 bit.

## Installazione

1. Chiudere AutoCAD.
2. Scaricare l'installer dalla sezione **Releases**.
3. Avviare `YQArch_Italiano_3.61.exe`.
4. Riaprire AutoCAD.
5. Eseguire `YQIT_DIAGNOSTICA_COMPLETA`.

Per installazioni legacy utilizzare il pacchetto ZIP e consultare `INSTALLAZIONE_LEGACY.md`.

## Verifica installazione

In AutoCAD sono disponibili:

- `YQIT_DIAGNOSTICA_COMPLETA` — verifica il caricamento del runtime e il registro dei 646 comandi;
- `YQIT_COMPATIBILITA` — mostra versione AutoCAD, piattaforma, LISPSYS e fascia di compatibilità.

## Integrità versione 3.61

- EXE SHA-256: `02d998016c8458a1a103d87b2bd6cda84dd23e4f58eca9d7f5a34e6d4a0fe7d9`
- ZIP SHA-256: `945e344474f58cd2b187ebd472502f5811604b103d5480124f1a5571a5629137`

## Documentazione

Nel repository sono disponibili le note di rilascio, la matrice di compatibilità e le istruzioni di installazione legacy. La guida completa è distribuita insieme alla release.

## Progetto originale

YQArch Italiano è una localizzazione e modernizzazione indipendente del progetto YQArch originale. Il progetto originale, i relativi autori e le relative risorse mantengono la propria identità e attribuzione.
