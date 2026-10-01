# Compatibilità AutoCAD / Windows — YQArch Italiano 3.73

## Evidenza disponibile

La release 3.73 è stata collaudata il 1 ottobre 2026 sul PC di riferimento con **AutoCAD 2026**. Installazione/aggiornamento, caricamento, Ribbon e inserimento diretto dei blocchi sono stati confermati funzionanti.

Il collaudo non viene esteso automaticamente a tutti i 646 comandi o ad altre combinazioni AutoCAD/Windows.

## Fasce AutoCAD

- **AutoCAD 2026 Windows — collaudo reale sul PC di riferimento.**
- **AutoCAD 2010–2025 e 2027 Windows — compatibilità progettata e controllata staticamente.** La Ribbon è prevista da `ACADVER >= 18.0`; non tutte le release sono state eseguite realmente.
- **AutoCAD 2007–2009 Windows — percorso legacy.** Menu/toolbar e installazione legacy; tutti i 195 blocchi del catalogo sono in formati leggibili da queste versioni.
- **AutoCAD 2004–2006 Windows — compatibilità legacy parziale.** 147/195 blocchi sono leggibili; 48 sono `AC1021` e richiedono AutoCAD 2007 o successivo. La 3.73 li intercetta prima dell'inserimento.

Il catalogo contiene **16 AC1009, 2 AC1014, 129 AC1018 e 48 AC1021**.

AutoCAD LT, AutoCAD per Mac e CAD alternativi non sono dichiarati compatibili da questo pacchetto.

## Windows e installer

`YQArch_Italiano_3.73.exe` è un eseguibile **Windows x64**. Utilizzare una combinazione AutoCAD/Windows supportata da Autodesk per la propria release. Per sistemi legacy o 32 bit usare lo ZIP e la procedura manuale; questo non costituisce certificazione del sistema.

L'EXE non è firmato Authenticode e SmartScreen può mostrare un avviso di reputazione.

## Sicurezza

YQArch Italiano 3.73 non disattiva `SECURELOAD` e non modifica automaticamente `TRUSTEDPATHS` o `LISPSYS`. Il CUI principale di AutoCAD non viene sostituito e le interfacce di altre applicazioni non vengono azzerate.

## Riferimenti Autodesk verificati il 1 ottobre 2026

- Formati DWG: https://www.autodesk.com/it/support/technical/article/caas/sfdcarticles/sfdcarticles/ITA/AutoCAD-drawing-file-format.html
- Codici versione DWG: https://www.autodesk.com/it/support/technical/article/caas/sfdcarticles/sfdcarticles/ITA/drawing-version-codes-for-autocad.html
- Requisiti AutoCAD 2027: https://help.autodesk.com/cloudhelp/2027/ENU/AutoCAD-ReleaseNotes/files/installation/INSTALLATION_REQUIREMENTS_AUTOCAD_2027.html
