# YQArch Italiano

Localizzazione e modernizzazione italiana gratuita di **YQArch per AutoCAD**.

**Versione corrente: 3.73**  
Release pubblicabile del **1 ottobre 2026**.

## Stato del progetto

- guida italiana con **646 schede** ricercabili;
- Ribbon con **10 pannelli** e **130 accessi diretti**;
- **23 categorie** e **547 voci** nelle espansioni;
- catalogo di **195 blocchi DWG** con 195 anteprime;
- inserimento blocchi in un solo passaggio: selezione → Inserisci → punto nel DWG → completamento;
- diagnostica integrata con `YQIT_DIAGNOSTICA_COMPLETA` e `YQIT_COMPATIBILITA`;
- core storico conservato quando stabile;
- `SECURELOAD`, `TRUSTEDPATHS` e il CUI principale non vengono disattivati o azzerati dall'installer.

## Collaudo della 3.73

La 3.73 è stata installata e collaudata sul PC di riferimento con **AutoCAD 2026**. Sono stati verificati l'aggiornamento, il caricamento, la Ribbon e l'inserimento diretto dei blocchi.

Il collaudo del PC di riferimento e i test automatici non equivalgono a una certificazione di tutti i 646 comandi né di ogni combinazione AutoCAD/Windows.

## Compatibilità

| Fascia | Versioni AutoCAD per Windows | Stato |
|---|---|---|
| Collaudo reale | AutoCAD 2026 | installazione/aggiornamento, Ribbon e inserimento blocchi verificati |
| Moderna | AutoCAD 2010–2025 e 2027 | compatibilità progettata e controllata staticamente; non tutte le release sono state eseguite realmente |
| Legacy | AutoCAD 2007–2009 | menu/toolbar e procedura legacy; tutti i 195 DWG del catalogo sono leggibili |
| Legacy parziale | AutoCAD 2004–2006 | 147/195 blocchi leggibili; 48 AC1021 richiedono AutoCAD 2007+ |

L'installer `YQArch_Italiano_3.73.exe` è un eseguibile **Windows x64**. Per sistemi legacy o 32 bit è disponibile lo ZIP con procedura manuale. La compatibilità del plugin non rende supportata una coppia AutoCAD/Windows che Autodesk non supporta.

AutoCAD LT, AutoCAD per Mac e CAD alternativi non sono dichiarati compatibili da questa distribuzione.

## Download

La release pubblica è distribuita direttamente dal sito del progetto:

- [Installer EXE 3.73](https://andreagiaquinto.it/downloads/yqarch/YQArch_Italiano_3.73.exe)
- [Pacchetto ZIP 3.73](https://andreagiaquinto.it/downloads/yqarch/YQArch_Italiano_3.73.zip)
- [Guida completa](https://andreagiaquinto.it/downloads/yqarch/YQArch_Italiano_3.73_GUIDA.html)
- [Pagina del progetto](https://andreagiaquinto.it/yqarch-italiano/)

Non è necessario installare versioni precedenti prima della 3.73.

## Integrità versione 3.73

- EXE SHA-256: `07165f6a941ebb4b97e4842d4cdf4a03a017bd433cda8a17eb8f7aa419c6280d`
- ZIP SHA-256: `ec14d087067620222a721da25c1034167edb9411741ac5fe5dc69ba76c839df2`

L'EXE non è firmato Authenticode; Windows può mostrare un avviso di reputazione. Verificare l'hash e non disattivare le protezioni di Windows o AutoCAD.

## Installazione

1. Chiudere tutte le sessioni di AutoCAD.
2. Scaricare l'EXE 3.73 dal sito.
3. Avviarlo con l'account Windows con cui viene usato AutoCAD.
4. Completare l'installazione/aggiornamento.
5. Riaprire AutoCAD ed eseguire `YQIT_DIAGNOSTICA_COMPLETA`.
6. Provare i comandi su una copia del DWG.

Per installazioni manuali o legacy consultare `INSTALLAZIONE_LEGACY.md`.

## Compatibilità del catalogo

I 195 DWG inclusi sono: **16 AC1009, 2 AC1014, 129 AC1018 e 48 AC1021**. AutoCAD 2004–2006 può leggere 147 file; i 48 AC1021 richiedono AutoCAD 2007 o successivo e la 3.73 li intercetta prima dell'inserimento.

## Progetto originale

YQArch Italiano è una localizzazione e modernizzazione indipendente del progetto YQArch originale. Il progetto originale, i relativi autori, AutoCAD e i rispettivi marchi mantengono la propria identità e titolarità.
