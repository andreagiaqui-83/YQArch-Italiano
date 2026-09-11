# Compatibilità AutoCAD / Windows — YQArch Italiano 3.61

## Fasce di compatibilità del plugin

- **Primaria:** AutoCAD 2021–2027 per Windows.
- **Estesa:** AutoCAD 2015–2020 per Windows. I moduli italiani LSP/DCL caricabili sono distribuiti in MBCS/Windows-1252 per mantenere la compatibilità con le versioni precedenti al nuovo ambiente AutoLISP Unicode.
- **Legacy:** AutoCAD 2008–2014, best effort.
- **Legacy parziale:** AutoCAD 2004–2007. Il core storico riconosce queste generazioni, ma non è corretto garantire tutti i 646 comandi senza collaudi reali.

## Installer

- `YQArch_Italiano_3.61.exe`: Windows 10/11 x64.
- Per sistemi precedenti o a 32 bit: usare il pacchetto ZIP portabile e la procedura manuale.

## Compatibilità ufficiale AutoCAD / Windows

La compatibilità del plugin non sostituisce i requisiti ufficiali Autodesk della singola versione di AutoCAD. Una combinazione AutoCAD/Windows non supportata da Autodesk non diventa supportata solo perché YQArch Italiano riesce tecnicamente a caricarsi.

L'ambiente reale di riferimento della 3.61 è **AutoCAD 2027 italiano su Windows 11 x64**.

## Diagnostica

- `YQIT_DIAGNOSTICA_COMPLETA` mostra versione AutoCAD, fascia plugin e stato dei 646 comandi.
- `YQIT_COMPATIBILITA` mostra `ACADVER`, piattaforma, LISPSYS/MBCS e fascia di compatibilità.

## Limiti della verifica

Le fasce estesa e legacy derivano da analisi tecnica/statica del codice e dei formati distribuiti. Non equivalgono a una certificazione runtime su ogni singola versione di AutoCAD.
