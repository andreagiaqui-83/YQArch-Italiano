# Installazione, aggiornamento e ripristino — YQArch Italiano 3.73

## Installazione normale con EXE
1. **Chiudere completamente AutoCAD.** Conservare almeno la 3.71 collaudata e una seconda baseline precedente come rollback.
2. Avviare `YQArch_Italiano_3.73.exe` con l'account Windows dell'utente che utilizza AutoCAD.
3. L'installer rileva i profili di **AutoCAD completo** e aggiorna soltanto i file distribuiti dal pacchetto. Non azzera il profilo, non sostituisce il CUI principale e non modifica BlockHub CAD o Express Tools.
4. I file personali già presenti nelle cartelle utente vengono preservati quando non appartengono al manifest del plugin. I file distribuiti che devono essere sostituiti vengono prima registrati nel journal e salvati nel backup locale.
5. Al termine avviare AutoCAD, aprire un DWG di prova e verificare: scheda **YQArch Italiano**, un comando dalla Ribbon, un inserimento dal catalogo e `YQIT_DIAGNOSTICA_COMPLETA`.

L'installer mostra avanzamento e operazioni in corso, porta la finestra in primo piano all'avvio e poi consente il normale uso/minimizzazione. Durante un aggiornamento evita di ricopiare file già identici e riutilizza le verifiche hash già completate, riducendo letture inutili senza eliminare i controlli d'integrità.

## ZIP / installazione manuale
Usare lo ZIP quando l'EXE x64 non è adatto al sistema oppure quando si preferisce una distribuzione manuale controllata.

1. Estrarre l'intero pacchetto in una cartella stabile e scrivibile.
2. La cartella principale del plugin è `YQArchItaliano\sys`.
3. Aggiungere questa cartella ai **Percorsi di ricerca dei file di supporto** del profilo AutoCAD interessato.
4. Configurare i percorsi attendibili soltanto se richiesto dalle policy del proprio ambiente. Non disattivare globalmente `SECURELOAD`.
5. Caricare `YQArchItaliano_Bootstrap.lsp` con `APPLOAD` e, se necessario, aggiungerlo al Gruppo di avvio.
6. Chiudere e riaprire AutoCAD, quindi verificare anche l'apertura di un secondo DWG.

Per AutoCAD 2004–2009 usare il percorso legacy menu/toolbar. La Ribbon 3.73 viene attivata soltanto da AutoCAD 2010 in poi.

## Limite dei blocchi su AutoCAD 2004–2006
Il catalogo standard contiene 195 DWG. **147** sono leggibili da AutoCAD 2004–2006; **48** sono in formato AutoCAD 2007 (`AC1021`). La 3.73 controlla l'intestazione del DWG prima dell'inserimento: su una release troppo vecchia mostra un messaggio di incompatibilità e non crea oggetti parziali o definizioni di blocco incomplete.

Questo controllo evita un errore operativo, ma non converte i 48 file. Per usarli realmente con AutoCAD 2004–2006 occorre una conversione legittima verso il formato AutoCAD 2004 effettuata con un prodotto compatibile/licenziato e poi un nuovo collaudo dei DWG convertiti.

## Aggiornamento manuale
Prima di sostituire una versione esistente:
- copiare l'intera cartella YQArch corrente in un backup;
- conservare i file personali non distribuiti dal pacchetto;
- sostituire soltanto i file del plugin;
- rimuovere/spostare nel backup le vecchie cache compilate del menu YQArch (`.mns`, `.mnc`, `.mnr`, `.cui`, `.cuix`) quando sono cache generate, **non** il CUIx Ribbon distribuito;
- non modificare `acad.cuix`, `acad.lsp`, `acaddoc.lsp` o gli equivalenti di versione se appartengono all'utente.

Se un `acad.lsp`/`acaddoc.lsp` personale è già in uso, aggiungere soltanto l'eventuale chiamata al bootstrap preservando integralmente le altre routine.

## Ripristino
In caso di errore o annullamento, l'installer tenta il rollback delle modifiche già eseguite. I backup e il journal restano nella cartella locale di YQArch Italiano. In caso di spegnimento imprevisto usare il journal, a AutoCAD chiuso, per ripristinare i file che esistevano e rimuovere esclusivamente quelli creati da quella installazione.

La 3.71 resta la baseline di rollback principale perché è stata collaudata sul PC di riferimento.

## File che devono restare insieme
Per il menu italiano mantenere insieme i file `YQArchItaliano_Menu_372.*` distribuiti. Per la Ribbon mantenere insieme `YQArchItaliano_Ribbon_372.cuix`, il relativo `.lsp/.mnl` e le risorse. Per il catalogo mantenere `YQArchItaliano_Library_372.lsp/.dcl`, `YQArchItaliano_Catalogo_372.*`, la cartella `blocks` e le anteprime.

Le preferenze personali del catalogo in `%LOCALAPPDATA%\YQArchItaliano\Catalogo` non devono essere eliminate durante un normale aggiornamento.