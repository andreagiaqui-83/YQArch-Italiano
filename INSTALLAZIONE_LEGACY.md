# Installazione manuale / legacy — YQArch Italiano 3.61

Questa procedura è destinata ai sistemi per i quali non è utilizzabile l'installer EXE corrente, in particolare installazioni Windows precedenti o AutoCAD a 32 bit.

1. Chiudere AutoCAD.
2. Estrarre integralmente `YQArch_Italiano_3.61.zip` in una cartella locale stabile.
3. Conservare intatta la struttura delle sottocartelle.
4. Aggiungere la cartella del plugin ai percorsi di supporto attendibili di AutoCAD secondo le impostazioni della propria versione.
5. Caricare il bootstrap YQArch previsto dal pacchetto.
6. Riavviare AutoCAD.
7. Eseguire `YQIT_DIAGNOSTICA_COMPLETA`.
8. Eseguire `YQIT_COMPATIBILITA` e verificare la fascia rilevata.

Non disattivare globalmente le protezioni `SECURELOAD` e non sostituire indiscriminatamente i percorsi attendibili esistenti.

Le versioni AutoCAD 2008–2014 sono considerate legacy/best effort; AutoCAD 2004–2007 è considerato legacy parziale. Per queste generazioni alcuni comandi possono dipendere da funzionalità AutoCAD introdotte successivamente.
