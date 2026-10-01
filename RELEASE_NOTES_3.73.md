# YQArch Italiano 3.73 — Note di rilascio

Release definitiva del 1 ottobre 2026.

## Correzione principale
La 3.72 poteva interrompersi durante l'aggiornamento di più profili AutoCAD a causa della collisione tra `$script:V` e `$v`: PowerShell non distingue maiuscole e minuscole nei nomi delle variabili. La 3.73 usa variabili distinte e un controllo `.ContainsKey()`, con test anti-regressione dedicato.

## Funzioni preservate
- Ribbon della 3.71: 10 pannelli, 3 icone grandi + 10 piccole per pannello, 130 accessi diretti.
- 23 categorie e 547 voci nelle espansioni.
- Inserimento blocchi: selezione → Inserisci → punto nel DWG → completamento.
- Backup, journal e rollback dell'installer.
- Guida con 646 schede.

## Miglioramenti
- controllo preventivo del formato DWG prima dell'inserimento;
- aggiornamento più rapido evitando hash duplicati sui file già verificati identici;
- pulizia limitata alle cache YQArch obsolete;
- documentazione e compatibilità aggiornate.

## Verifiche
- 184/184 test logici/API simulate/regressioni: PASS;
- 71/71 controlli statici/risorse: PASS;
- 31/31 controlli di packaging: PASS;
- suite ripetute sul vero EXE estratto: PASS;
- seconda ricostruzione EXE/ZIP byte-identica;
- collaudo reale sul PC di riferimento con AutoCAD 2026: installazione/aggiornamento, Ribbon e inserimento blocchi PASS.

Questi risultati non costituiscono certificazione Autodesk né un collaudo di ogni comando su ogni versione AutoCAD/Windows.

## Hash
- EXE: `07165f6a941ebb4b97e4842d4cdf4a03a017bd433cda8a17eb8f7aa419c6280d`
- ZIP: `ec14d087067620222a721da25c1034167edb9411741ac5fe5dc69ba76c839df2`

La 3.72 non deve essere distribuita. La 3.71 resta la baseline di rollback collaudata.
