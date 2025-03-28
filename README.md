# Analisi sulla Leucemia in Europa (1990–2021): Epidemiologia e Mercato Farmaceutico

### 1. Descrizione del progetto
Questo progetto rappresenta una simulazione di analisi sull’industria dell’healthcare, con focus specifico sul mercato europeo della leucemia (dal 1990 al 2021).
L’obiettivo principale è la gestione dei dati end-to-end, dalla fase di ETL (Extract, Transform, Load) fino alla modellazione e visualizzazione in Power BI, offrendo una panoramica delle best practices per la preparazione, la modellazione e la presentazione dei dati, attraverso un data cleaning in Python e una configurazione pulita e piacevole in Power BI.

(Tutti i files che compongono il progetto sono caricati in una cartella su Google Drive a questo link:
https://drive.google.com/drive/folders/1NPbewN9RaPXhF2U66D_Kj7F-rPQrZWxS?hl=it)

### 2. Struttura del progetto
Cartella “Raw Data”: contiene i dataset originali così come sono stati reperiti (file .csv e .xlsx).
Cartella “Final Data”: include i dataset puliti e pronti per l’uso in Power BI, frutto delle operazioni di ETL.
File "Python Scripts.ipynb": Jupyter Notebook con tutti gli script di ETL realizzati in Python (pandas, ecc.). Contiene commenti che descrivono le operazioni di pulizia, normalizzazione e selezione dei dati.
File "Leukemia Analysis - PowerBi Report.pbix": il report finale creato in Power BI, comprensivo di tutte le visualizzazioni interattive, i calcoli DAX e la modellazione.
File "Leukemia Analysis.pdf": una copia statica del report esportata da Power BI, per una consultazione rapida senza necessità di aprire il file .pbix.


### 4. Dataset e fonti
Dati epidemiologici: derivano dall’Università di Washington, con statistiche mondiali (e poi focalizzate sull’Europa) sulla mortalità, incidenza e prevalenza della leucemia.
Dati di mercato: ottenuti tramite “Deep Research” di ChatGPT e rifiniti come sample data realistici, poiché non erano disponibili dati ufficiali per la medesima finestra temporale.
I file sono in formato .csv e .xlsx; alcuni valori sono stime o simulazioni a scopo dimostrativo.


### 5. Metodologia
#### Fase di ETL (in Python):
Estrazione dei dati da diverse fonti (file raw).
Trasformazione: pulizia, standardizzazione dei formati e selezione delle variabili di interesse.
Caricamento dei dataset riformattati nella cartella “Final Data” per l’utilizzo in Power BI.

#### Modellazione in Power BI:
Creazione di uno Star Schema (tabelle di fatti e dimensioni) per avere un modello semantico semplice ed efficiente.
Sviluppo delle misure DAX necessarie all'analisi mantenendo come obiettivo il rapporto performance/interattività.

#### Visualizzazioni:
Dashboard interattive con slicer (filtri per anno, Paese, tipologia di leucemia, misura).
Bottoni e bookmarks per navigare tra diverse viste tematiche.
Elementi testuali dinamici per presentare i dati in modo immediato.
