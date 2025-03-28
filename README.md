# Something in the air
Questo repository contiene i dati del progetto **Something in the air**, una mappatura dei picchi orari di benzene registrati in Italia tra 2013 e 2023. 
Per picco di benzene s'intende una concentrazione media oraria di benzene nell'aria maggiore della soglia critica di 27 microgrammi/metro cubo. 

## 📖Contesto
Quando le concentrazioni di benzene nell'aria sono un pericolo per salute?

La [direttiva UE 2008/EC/50](https://eur-lex.europa.eu/eli/dir/2008/50/oj/ita/pdf) sulla qualità dell'aria fissa a 5 µg/m³ (microgrammi/metro cubo) la soglia della media annuale concentrazione del benzene (C6H6) nell'aria, ma non stabilisce un limite per le concentrazioni orarie. In letteratura, si considera la soglia di 27 µg/m³ significativa ai fini degli effetti avversi sulla salute. Tale limite viene preso come riferimento nella [normativa californiana](https://oehha.ca.gov/chemicals/benzene). Quindi, la popolazione di un territorio con una media annuale di benzene considerata accettabile (< 5 µg/m³), potrebbe avere comunque effetti avversi sulla salute se i dati orari dietro quella media presentano picchi di benzene critici (>27 µg/m³).

Il progetto vuole quindi individuare dove in Italia si sono registrati picchi orari di benzene superiori alla soglia critica.

### 📊Taranto, un caso studio di interesse
Questa ricerca prende ispirazione dall'[analisi sui picchi orari di benzene a Taranto](https://www.isdenews.it/i-picchi-di-benzene-a-taranto/), presentata in Senato dall'associazione Peacelink nel febbraio 2024. I dati presentati da Peacelink sono stati raccolti dal [software Ominscope](https://www.peacelink.it/ariataranto), che ha analizzato le medie orarie del benzene nella centralina ARPA di via Machiavelli del quartiere Tamburi di Taranto tra 2013 e 2023.




## 🔍Fonti e metodologia

### 📌[MAPPATURA PICCHI BENZENE.csv](https://github.com/schenzio/picchi_benzene/blob/main/MAPPATURA%20PICCHI%20BENZENE.csv)
Il file *MAPPATURA PICCHI BENZENE.csv* è costruito da un'elaborazione dei dati dall'[Environmental European Agency](https://eeadmz1-downloads-webapp.azurewebsites.net/). 
Ogni record del file è una rilevazione di un picco orario di benzene registrato da una stazione di monitoraggio dell'aria. 
Per ogni picco, sono indicati:

- **ID** – Identificatore unico della stazione di monitoraggio.
- **Inizio** (YYYY-MM-DD h:min:s) – Data e ora di inizio della rilevazione del picco di benzene.
- **Inizio** (DD/MM/YYYY) – Data di inizio della rilevazione, in formato giorno/mese/anno.
- **Fine** (YYYY-MM-DD h:min:s) – Data e ora di fine della rilevazione del picco di benzene.
- **Fine** (DD/MM/YYYY) – Data di fine della rilevazione, in formato giorno/mese/anno.
- **Year** – Anno della rilevazione.
- **Value (μg.m-3)** – Concentrazione di benzene registrata (in microgrammi per metro cubo).
- **Comune** – Comune in cui è situata la stazione di rilevazione.
- **Indirizzo** – Indirizzo della stazione di monitoraggio.
- **Air Quality Station Area** – Tipologia dell’area in cui si trova la stazione (rural, suburban, urban).
- **Latitudine** – Coordinate geografiche di latidudine della stazione
- **Longitudine** – Coordinate geografiche di longitudine della stazione.
- **EOL Code stazione** – Codice identificativo EOL della stazione di monitoraggio.
- **Tipo stazione** – Tipologia della stazione (es. industriale, fondo, traffico).
- **Provincia** – Sigla della provincia in cui è situata la stazione.
- **Provincia (nome completo)** – Nome esteso della provincia in cui è situata la stazione.
- **Regione** – Regione italiana in cui è situata la stazione.
- **Area** – Area geografica (Nord-est, Nord-ovest, Centro, Sud, Isole) della stazione.
- **Area (macro)** – Macro area geografica (Nord, Centro, Sud e isole) della stazione.

### 📌[Notebook](https://github.com/schenzio/picchi_benzene/blob/main/Notebook_Something_in_the_air.ipynb)
Il file *Notebook_Something_in_the_air.ipynb* contiene contesto istruzioni e codice python per riprodurre il lavoro, a partire scaricati dall'Environamental e pubblicati nella cartella [EEA_data](https://github.com/schenzio/picchi_benzene/tree/main/EEA_data)
