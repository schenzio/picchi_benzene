# Something in the air - Mappatura dei picchi di benzene
Questo repository contiene i dati del progetto **Something in the air**, una mappatura dei picchi orari di benzene registrati in Italia tra 2013 e 2023. 
Per picco di benzene s'intende una concentrazione media oraria di benzene nell'aria maggiore della soglia critica di 27 microgrammi/metro cubo. 


I dati sono contenuti nel file *MAPPATURA PICCHI BENZENE.csv*, costruito da un'elaborazione dei dati dall'Agenzia Ambientale Europea. 
Ogni record del file è una rilevazione di un picco orario di benzene registrato da una stazione di monitoraggio dell'aria. 
Per ogni picco, sono noti:

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


Nella cartella metodologia, è disponibile un notebook con le istruzioni su come ricostruire il file.
