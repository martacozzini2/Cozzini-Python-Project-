**##HumanVsMachineTextClassifier**

**##Description**

Il progetto implementa un classificatore in grado di distinguere tra testi scritti da umani e testi generati da modelli di linguaggio automatizzati (come GPT). 
Nella prima parte del codice si utilizzano tecniche di Natural Language Processing (NLP) per estrarre feature significative dai testi, come il numero di token, la lunghezza delle frasi, il numero di verbi, ecc. Dopo aver estratto le feature significative viene addestrato un classificatore per distinguere tra le due categorie. 
Il classificatore è composto da: un'architettura LSTM per l'elaborazione del testo, un'analisi delle feature numeriche, un layer di concatenazione per combinare i dati testuali e numerici e un layer fully connected per la classificazione finale. 
Nell'ultima parte del codice si utilizza LIME viene per esplorare e interpretare il comportamento del modello, migliorando la comprensione delle decisioni prese dal classificatore.

**##Dataset**

Il dataset utilizzato in questo progetto non è incluso direttamente nella repository, ma può essere trovato su Google Drive. Per poter utilizzare il modello, è necessario scaricare o montare il dataset da questo link https://drive.google.com/file/d/1vevvCWhiFrkcLfNQs4CUHrUWFOzj-uB7/view?usp=sharing

Il dataset contiene un totale di 50.000 testi. Tuttavia, per motivi di memoria e spazio, si è deciso di utilizzare solo una parte di questo, pari a 15.000 testi. Di questi, 7.500 sono scritti da esseri umani e 7.500 sono generati da macchine. I testi sono suddivisi in due classi: "human" e "ai".

**##Struttura del progetto** 

Il progetto è suddiviso in tre parti principali, ma tutto il codice è contenuto in un unico file [main.py ](/main.py) i risultati generati dal modello sono salvati in una cartella denominata [results](/results) che contiene tre sottocartelle:

-features: risultati dell'estrazione delle caratteristiche

-performance: performance del classificatore (accuratezza, matrice di confusione, ecc.)

-lime analysis: spiegazioni fornite da LIME per alcuni testi


**##Requirements**

Python 3.x

Le librerie Python necessarie sono elencate nel file [requirements.txt](/requirements.txt) 

**##Usage**

Scarica il dataset e caricalo nel tuo ambiente di programmazione.

Una volta configurato l'ambiente, esegui il file [main.py](/main.py) con il comando `python main.py` per avviare il progetto







