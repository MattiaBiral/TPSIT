# Programmazione Concorrente

- **Programma**:  
Contiene  le istruzioni che dovranno essere eseguite, è un' entità passiva
- **Processo**:  
Programma in esecuzione, entità logica in evoluzione
  - Cooperante: influenza o può essere influenzato da altri processi in esecuzione nel sistema producendo/utilizzando dati in condivisione con altri processi
  - In competizione: può evolvere indipendentemente ma entra in conflitto sulla ripartizione delle risorse
- **Processo Control Block**:
  - Process IDentifier
  - Stato
  - Contesto
    - Program Counter
    - Registri
  - Priorità
  - Limiti di memoria
  - Risorse allocate
- **Sistema multiprogrammato**:  
Può eseguire più processi contemporaneamente
- **Processo Indipendente**:  
Non necessita di risorse utilizzate da altri processi
- **Stati di un processo**:
  - New
  - Running
  - Ready
  - Waiting
  - Terminated
- **Risorsa**:  
Componente hardware o software necessario ad un processo per evolvere
- **Istanza**:  
Risorsa di una classe
- **Molteplicità**:  
Il numero di risorse di una classe
- **Classificazione di risorse e processi**:
  - Richieste
    - Numero
      - Singola
      - Multipla
    - Tipo
      - Bloccante
      - Non bloccante
  - Assegnazione
    - Statica
    - Dinamica
- **Classificazione delle risorse**:
  - Esclusività:
    - Seriale
    - Non seriale
  - Utilizzo
    - Prerilasciabile
    - Non prerilasciabile
- **Grafo di Holt**:
  - Simboli
    - Quandrato -> Risorsa
    - Cerchio -> Processo
    - Freccia verde da risorsa a processo -> assegnata
    - Freccia rossa da processo a risorsa -> richiesta, non disponibile
  - **Riducibile**:  
  C'è almeno un processo con solo frecce entranti
- **Thread**:  
Flusso di controllo che può essere attivato in parallelo ad altri thread nell'ambito di uno stesso processo e quindi nell'esecuzione dello stesso programma, condivide le risorse con gli altri thread del processo
- **Multithreading**:  
Più thread possono essere eseguiti contemporaneamente
- **Thread Control Block**:  
Contiene le stesse informazioni del PCB, più
  - Spazio di memoria per le variabili locali
  - Puntatore al PCB del processo padre
- **Thread safety**:  
Nessun thread può accedere a dati mentre sono modificati/aggiornati
- **Stati di un thread**:  
Quelli di un processo più
  - Waiting -> Blocked
  - Sleping
  - Waiting
- **Fork-Join**:
  - Fork: creazione di un processo che inizia la propria esecuzione in parallelo con quella del processo chiamante
  - Join: viene eseguita quando il processo creato tramite la fork ha terminato il suo compito, si sincronizza con il processo che lo ha creato e termina la sua esecuzione