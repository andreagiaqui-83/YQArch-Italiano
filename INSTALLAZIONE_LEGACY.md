# Installazione manuale / legacy — YQArch Italiano 3.73

Questa procedura è destinata ai sistemi sui quali non è utilizzabile l'installer EXE x64 corrente o quando si preferisce una configurazione manuale.

1. Chiudere tutte le sessioni di AutoCAD.
2. Estrarre integralmente `YQArch_Italiano_3.73.zip` in una cartella locale stabile.
3. Conservare intatta la struttura delle sottocartelle.
4. Aggiungere la cartella del plugin ai percorsi di supporto/attendibili secondo le impostazioni della propria versione di AutoCAD.
5. Caricare il bootstrap YQArch indicato nella guida inclusa.
6. Riavviare AutoCAD.
7. Eseguire `YQIT_DIAGNOSTICA_COMPLETA`.
8. Eseguire `YQIT_COMPATIBILITA` e controllare la fascia rilevata.

Non disattivare globalmente `SECURELOAD`, non azzerare `TRUSTEDPATHS` e non sostituire indiscriminatamente i file personali `acad.lsp` o `acaddoc.lsp`.

## Versioni legacy

- AutoCAD 2007–2009: percorso legacy; i 195 DWG del catalogo sono in formati leggibili.
- AutoCAD 2004–2006: 147/195 blocchi sono leggibili; 48 file `AC1021` richiedono AutoCAD 2007+. La 3.73 segnala il limite prima dell'inserimento.

L'installazione manuale non costituisce una certificazione di ogni vecchia combinazione AutoCAD/Windows.
