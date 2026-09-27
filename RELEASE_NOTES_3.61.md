# YQArch Italiano 3.61

Versione pubblica aggiornata di YQArch Italiano.

## Novità principali

- verifica e documentazione della compatibilità AutoCAD/Windows;
- diagnostica estesa con `ACADVER`, anno AutoCAD, fascia di compatibilità e `LISPSYS`/MBCS;
- nuovo comando `YQIT_COMPATIBILITA`;
- moduli italiani LSP/DCL salvati in Windows-1252/MBCS quando possibile per mantenere la compatibilità con AutoCAD 2020 e precedenti;
- corretti riferimenti versione obsoleti nel runtime;
- documentata la differenza tra compatibilità del plugin e compatibilità ufficiale AutoCAD/Windows;
- aggiunta procedura portabile/manuale per sistemi legacy e 32 bit;
- mantenuti invariati i comandi geometrici già collaudati.

## Verifiche

- registro: **646/646 comandi definiti**;
- ambiente di riferimento reale: **AutoCAD 2027 italiano su Windows 11 x64**;
- diagnostica `YQIT_DIAGNOSTICA_COMPLETA`: positiva;
- diagnostica `YQIT_COMPATIBILITA`: positiva.

## SHA-256

- `YQArch_Italiano_3.61.exe`: `02d998016c8458a1a103d87b2bd6cda84dd23e4f58eca9d7f5a34e6d4a0fe7d9`
- `YQArch_Italiano_3.61.zip`: `945e344474f58cd2b187ebd472502f5811604b103d5480124f1a5571a5629137`
