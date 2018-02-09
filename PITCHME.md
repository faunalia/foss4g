# QGIS 3: novità e sviluppo


*Matteo Ghetta* matteo.ghetta@faunalia.eu

[Faunalia](https://www.faunalia.eu) e [QGIS IT](https://www.qgis.it)

FOSS4G-IT-2018 Roma, 21/02/2018

---?image=assets/qgis3.png&size=contain

---


## Perché QGIS3

* aggiornamento librerie di base

    * **Qt4** -> **Qt5**
    * **python2** -> **python3**

* mantenimento nel tempo
* codice più chiaro
* nuove funzionalità

* pulizia codice QGIS3 stesso (*API break*)


---

## Cosa è stato fatto (1)

- Migrazione a Qt5 e Python 3 completata
- Helper per la migrazione dei plugins da Python 2 a 3
- Ristrutturazione delle proprietà dei layer: codice modulare
- *Task manager* per la gestione dei processi lunghi

---?image=assets/taskmanager.png&size=contain


---

## Cosa è stato fatto (1)

* <span style="color:gray">Migrazione a Qt5 e Python 3 completata</span>
* <span style="color:gray">Helper per la migrazione dei plugins da Python 2 a 3</span>
* <span style="color:gray">Ristrutturazione delle proprietà dei layer: codice modulare</span>
* <span style="color:gray">*Task manager* per la gestione dei processi lunghi</span>
* supporto nativo per 3D

---?image=assets/3d.png&size=contain


---

## Cosa è stato fatto (2)

* [Profili utente e impostazioni unificate](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/82)
* [Ridisegno dell'interfaccia utente per campi, widgets e moduli](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/37)

    * chiara separazione fra la gestione dei campi e i moduli

* [Ristrutturazione di QGIS server](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/74)
* [Strumento vertici migliorato](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/69)
* [Mappe multiple in un solo progetto](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/70)

---?image=assets/multimappe.png&size=contain

---

## Cosa è stato fatto (3)

* [Ristrutturazione del sistema di stampa](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/39)
* [Stampa di report complessi](https://north-road.com/qgis-layout-and-reporting-engine-campaign/)
* [Miglioramenti alla gestione dei metadati](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/50)
* [Sistema di help unificato](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/51)
* [Documentazione algoritmi Processing](http://blog.qgis.org/2017/04/30/qgis-grant-programme-2-results/)
* molte altri miglioramenti *nascosti*

---?image=assets/processing_help.png&size=contain

---


## Cose ancora da fare

* [Ristrutturazione del registro dei layer e legenda](https://github.com/qgis/QGIS-Enhancement-Proposals/issues/76)

  * aprire >1 progetto simultaneamente
  * migliore gestione dei layers embedded

* Continuare *Porting* algoritmi Processing in `C++`
* [Miglioramento supporto 3D](https://www.lutraconsulting.co.uk/crowdfunding/more-qgis-3d/)

    * supporto mappe 3D in layout di stampa
    * supporto per animazioni stile *telecamera*

---

## Chi sta pagando per tutto questo?

* Sponsors e donors

  * [QGIS Grants](https://www.qgis.org)

* QUGs: soprattutto QGIS.CH
* Aziende che ci tengono al futuro di [QGIS](https://www.qgis.org)
* Lavoro volontario

---

## Cosa rimane da fare

* Backup e versionamento dei files di progetto
* Miglioramenti a Processing
* Maggior numero di test
* Documentazione completa dei cambiamenti delle API

* [Una lista completa](https://github.com/qgis/QGIS-Enhancement-Proposals/issues)


---

## Cosa c'è di nuovo per gli sviluppatori

* Un ambiente di lavoro più confortevole

  * codice più pulito
  * librerie più moderne

* Ulteriori sviluppi più facili e rapidi

---

## Cosa c'è di nuovo per gli utenti - 1

* Nessuna rivoluzione, ma >100 novità:

  * Stili

    * nuove funzioni per le espressioni
    * point cluster renderer
    * **tutta** la stilizzazione è ora parametrizzabile con le espressioni
    * gestione dei simboli personalizzati più facile
    * annotazioni con stili parametrizzati

---

## Cosa c'è di nuovo per gli utenti - 2


* Analisi

    * riproiezione al volo sempre attiva
    * correzione topologia durante le analisi
    * algoritmi per il calcolo dei network
    * vari altri algoritmi
    * plugins (heatmap, zonal stats, ecc.) spostati in Processing
    * miglioramenti del modeler

---

## Cosa c'è di nuovo per gli utenti - 3

* Altro

    * gestione più furba visibilità dei layers nei gruppi
    * nascondi i layer deselezionati
    * [refresh automatico della mappa](https://www.youtube.com/watch?v=TQTfpiyUwXk&feature=youtu.be)
    * [refresh più veloce per progetti con etichette](https://github.com/qgis/QGIS/pull/4110)
    * miglioramenti nella gestione dei moduli
    * constraints, autocompletamento, ecc.
    * editing diretto dei raster

---

## Cosa c'è di nuovo per gli utenti - 4

* Altro

    * misurazione più precise
    * server più veloce (multithread)

* [una lista più completa](https://gist.github.com/nyalldawson/95738ec265c7f9bdb64b15672c210bb7)
* grafici D3 interattivi con DataPlotly

---?image=assets/dataplotly.gif&size=contain

---

## Quando aggiornare i tuoi plugins?


* Iniziare ora

    * plugin di compatibilità 2 --> 3

* *freeze* fatto. lavoro può iniziare

    * le API cambieranno ancora, in modo incrementale

* già >80 plugin disponibili (nuovi o *portati*)

---

## Cosa puoi fare

* Testing
* Documentazione
* Traduzione
* Sviluppo
* Sostenere il lavoro degli sviluppatori

---

## Si ma quando?!

Presto!

**Rilascio imminente** 2018-02-23 durante HF Madeira

---


## Licenza di questa presentazione


Creative Commons
Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)

![](https://upload.wikimedia.org/wikipedia/commons/d/d0/CC-BY-SA_icon.svg)

* More info: http://creativecommons.org/licenses/by-sa/3.0/
