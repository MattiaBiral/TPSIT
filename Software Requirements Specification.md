# Specifica dei requisiti

## Studio di fattibilità
Valutazione preliminare di costi e benefici, si stabilisce se è conveniente avviare il progetto.
Generalmente si conclude con la presentazione di un'offerta al cliente

## Specifica dei requisiti
- **Analisi del problema**: comprendere cosa deve fare il sistema
- **Definizione delle funzionalità**: ogni caratteristica richiesta per soddisfare le necessità del cliente
- **Redazione del documento di Specifica dei Requisiti Software**: documento formalizzato che raccoglie le specifiche tecniche e funzionali
- **Convalida delle specifiche**: il SRS viene analizzato e rivisto con il committente per validare ogni singola specifica

> ### Requisito
> Proprietà richiesta oppure auspicabile di un prodotto

> ### Stakeholder
> Tutte le persone in qualche modo interessate alla messa in opera del sistema, coinvolte nella raccolta dei requisiti

I **requisiti** possono cambiare sia durante la fase di **analisi** che in tutto il ciclo di **sviluppo**

## Classificazione dei requisiti
- Livello di dettaglio
  - Utente
  - Sistema
- Tipo di requisito
  - Funzionale
  - Non funzionale
  - Di dominio

> ### Requisiti funzionali
> Descrivono le funzionalità che il sistema deve avere, devono essere
> - **Completi**: indicare tutti i servizi richiesti
> - **Coerenti**: non devono avere definizioni contraddittorie

> ### Requisiti non funzionali
> Sono imposti dalle modalità operative, da una legge, uno standard o una best practice. Il sistema deve rispettare questi vincoli perché imposti dall'organizzazione o dall'esterno

> ### Requisiti di dominio
> Sono dipendenti dal dominio in cui il sistema deve operare.
> Esempi: la riservatezza dei dati sensibili, il login.

### Modello FURPS
- **Functionality**: funzioni fornite
- **Usability**: semplicità di apprendimento e utilizzo del sistema
- **Reliability**: garantire nel tempo le funzioni richieste per un range di situazioni e fornire risposte sempre corrette
- **Performance**: tempo di risposta del sistema
- **Supportability**: adattabilità del sistema alle modifiche

### Vincoli
- **Implementazione**: vincoli sull'implementazione del sistema
- **Interfacce**: vincoli imposti da sistemi esterni, inculso sistemi di legacy e formati di cambio
- **Operazioni** vincoli sull'amministrazione e sulla gestione del sistema
- **Packaging**: vincoli sulla consegna del sistema
- **Legali**: licenze, regolamentazioni e certificazioni

## Verifica e validazione dei requisiti
I requisiti **funzionali** sono abbastanza semplici da verificare, si effettua il collaudo con gli utilizzatori, si controllano:
- **Correttezza**: rappresenta perfettamente il sistema che viene richiesto
- **Completezza**: contempla tutti i possibili scenari
- **Coerenza**: i requisiti non si contraddicono
- **Chiarezza**: non ci sono possibili interpretazioni
- **Realismo**: deve essere realizzabile
- **Verificabilità**: deve essere possibile eseguire tutti i test
- **Tracciabilità**: tutte le funzioni devono essere individuabili

I requisiti di **dominio** possono essere verificati collaudando le interazioni del sistema

I requisiti **non funzionali** possono risultare non quantificabili e difficili da verificare, è generalmente possibile dare un valore quantitativo del grado di soddisfacimento

# Raccolta e analisi dei requisiti

La raccolta e analisi dei requisiti prende anche il nome di **fase di esplorazione**

## Tipi di realizzazione
- **Greenfield engineering**: lo sviluppo parte da zero, la fonte dei requisiti è il committente
- **Re-engineering**: esiste già un sistema che deve essere riprogettato, l'analisi del sistema esistente è alla base del nuovo progetto
- **Interface engineering**: non è necessario raccogliere nuovi requisiti in quanto viene fatta soltanto una riprogettazione delle interfacce

La raccolta dei requisiti dagli stakeholder viene anche chiamata **requirement elicitation**

## Tecniche di esplorazione
- **Interviste individuali**: l'intervistatore può controllare il flusso dell'intervista ma richiede molto tempo, possono essere:
  - Strutturate
  - Non strutturate
  - Semi-strutturate
- **Focus group**: servono a mettere a fuoco un determinato argomento, fanno emergere le aree di conflitto e di consenso ma richiedono esperienza
- **Osservazioni sul campo**: servono a comprendere il contesto, permettono di ottenere una consapevolezza dell'uso reale del prodotto ma richiedono tempo e risorse
- **Suggerimenti spontanei degli utenti**: hanno bassi costi di raccolta e possono essere molto specifici
- **Questionari**: si possono raggiungere molte persone con poco sforzo ma vanno progettati con grande accuratezza, sono composti da un'insieme di domande con 5 risposte (scala di Likert)
- **Analisi della concorrenza e delle best practice**: si possono individuare soluzioni migliori adatte al settore
- **Scenari e casi d'uso**: descrivono ogni singola operazione che il sistema deve effettuare

La fase di esplorazione presenta delle **difficoltà** che possono essere suddivise in quattro tipologie:
- **Problemi d'ambito**: è difficile individuare il livello di dettaglio e di approfondimento che deve essere rispettato
- **Problemi di comprensione**
- **Problemi di conflitto**: il medesimo requisito può essere descritto in modo differente da stakeholder che appartengono a gruppi diversi
- **Problemi di volatilità**: i requisiti individuati non rimangono stabili per tutto il ciclo di vita del progetto

# Attori, casi d'uso e scenari

> ### Attore
> Chi o che cosa svolge l'azione, con attori si indicano tutte le entità che interagiscono con il sistema

> ### Caso d'uso
> Che cosa viene fatto, i casi d'uso sono le funzionalità che il sistema mette a disposizione, è avviato da un'attore e si conclude con successo quando l'obiettivo è raggiunto

> ### Scenario
> Rappresenta una particolare interazione tra uno o più attori e il sistema

## Tipi di scenari
- **As-is scenario**: la situazione attuale esistente nell'organizzazione, solitamente viene utilizzato durante il re-engineering
- **Visionary scenario**: viene utilizzato solitamente da committente in caso di greenfield egineering o nel re-engineering per descrivere il sistema futuro o desiderato
- **Evaluation scenario**: task che gli utenti dovrebbero svolgere nel sistema per i quali sarà poi valutato
- **Training scenario**: tutorial che indica passo passo come un neofita può imparare il corretto utilizzo del sistema

Tra un **attore** e un **caso d'uso** viene indicata l'associazione mediante un segmento che li congiungie indicando una o più delle possibili situazioni:
- L'attore esegue il caso d'uso
- L'attore fornisce informazioni al caso d'uso
- L'attore riceve informazioni dal caso d'uso

## Relazioni tra casi d'uso
- **Inclusione**: un caso d'uso ne utilizza un'altro
- **Estensione**: aggiunge dei passi ad un caso esistente
- **Generalizzazione**: un caso d'uso eredita caratteristiche da un altro caso d'uso

## User stories del modello agile
Nei modelli agili i requisiti si scrivono mediante le **user stories**, composte da tre parti:
- Situazione (as a)
- Motivazione (i want)
- Aspettativa (so that)

# La documentazione dei requisiti

## Generalità
Il lavoro di individuazione dei requisiti termina con la stesura del documento di **Specifica dei Requisiti Software**.
Esistono tre tipologie di informazioni:
- Analisi degli **utenti**:
  - Categorie
  - Caratteristiche e priorità
- Analisi dei **bisogni**:
  - Necessità di ciascuna categoria di utenti
  - Quelli prioritari
- Analisi del **contesto d'uso**:
  - Diversi contesti d'uso del prodotto
  - Quelli prioritari

Nell'SRS vengono racolti in modo organizzato i requisiti individuati e come ha avuto luogo la loro determinazione

## RD proposto da Sommerville
- **Introduzione**
  - Scopo del prodotto
- **Definizione generale**
  - Prospettive
  - Funzioni
  - Caratteristiche degli utenti
  - Vincoli
  - Assunzioni e dipendenze
- **Requisiti specifici**
  - Requisiti funzionali
  - Requisiti non funzionali
  - Requisiti di sistema
- **Appendici**
  - Eventuale descrizione della piattaforma hardware
  - Requisiti di DataBase
  - Piani di Test
- **Indici**

All'interno del documento vengono utilizzati i seguenti termini IEEE:
- **Contratto**: documento legale stilato tracommittente e fornitore
- **Committente**: colui che paga il prodotto
- **Fornitore**: chi produce il prodotto
- **Utente**: la persona che usa e interagisce con il sistema

> Il documento SRS riporta in modo **corretto** e **non ambiguo** le specifiche dei requisiti ma non descrive **alcun dettaglio implementativo**

## Validazione dei requisiti
La validazione dei requisiti richiede di controllare:
- **Correttezza**: il sistema software soddisfa appieno ciascun requisito in esso riportato, una specifica è corretta se rappresenta accuratamente il sistema che il cliente richiede
- **Completezza**: tutti i possibili scenari per il sistema sono descritti
- **Consistenza**: i requisiti non devono essere in conflitto
- **Coerenza**: i requisiti non devono contraddirsi
- **Chiarezza**: non ci devono essere interpretazioni
- **Realismo**: una specifica deve poter essere implementata tenendo conto dei vincoli presenti
- **Modificabilità**: la struttura e lo stile devono essere tali da consentire facili modifiche
- **Verificabilità**: una specifica è verificabile se test ripetuti possono essere delineati per dimostrare che il sistema soddisfa i requisiti
- **Tracciabilità**: è necessario tracciare le dipendenze tra i requisiti e le funzioni del sistema.

## La convalida delle specifiche
I tipi di errori più frequenti sono:
- **Requisiti non chiari**: espressi male o informazioni omesse
- **Informazioni mancanti**: le informazioni mancano dal RD
- **Conflitto tra requisiti**: sono presenti contraddizioni
- **Requisiti non realistici**