### User Requirements Specification Document

##### DIBRIS – Università di Genova. Scuola Politecnica, Software Engineering Course 80154

**VERSION : X.X**

**Authors**  
XXXX
YYYY

**REVISION HISTORY**

| Version | Date | Authors | Notes |
| ------- | ---- | ------- | ----- |
| X.X     |      |         |       |

# Table of Contents

1. [Introduction](#p1)
   1. [Document Scope](#sp1.1)
   2. [Definitios and Acronym](#sp1.2)
   3. [References](#sp1.3)
2. [System Description](#p2)
   1. [Context and Motivation](#sp2.1)
   2. [Project Objectives](#sp2.2)
3. [Requirement](#p3)
   1. [Stakeholders](#sp3.1)
   2. [Functional Requirements](#sp3.2)
   3. [Non-Functional Requirements](#sp3.3)

<a name="p1"></a>

## 1. Introduction

<a name="sp1.1"></a>

### 1.1 Document Scope

<a name="sp1.2"></a>

### 1.2 Definitios and Acronym

| Acronym | Definition |
| ------- | ---------- |
| XXXX    | XXXX       |

<a name="sp1.3"></a>

### 1.3 References

<a name="p2"></a>

## 2. System Description

<a name="sp2.15"></a>

### 2.1 Context and Motivation

<a name="sp2.2"></a>

Si progetti un software per il controllo di un ATM il quale ha un lettore di
carte magnetiche, una console (tastiera e monitor) per interagire con
il cliente, un cassetto per depositare delle buste, un distributore di
banconote (in multipli di 20) una stampante per stampare le ricevute
per il cliente, uno switch che permette di operare in modalita'
operatore per accendere e spegnere la macchina. L'ATM comunichera'
con la banca tramite una connessione sicura, che pero' non fa' parte
del sistema che vogliamo progettare. L'ATM dovra' servire un cliente
alla volta, e ad ogni utente sara' richiesto di inserire la carta e il suo
PIN, i quali saranno spediti alla banca per la validazione come parte di
ogni transazione. Il cliente non avra' limiti di operazioni, ma la carta
rimarra' nell'ATM fino a quando il cliente indichera' di non voler piu'
eseguire operazioni. A quel punto verra' restituita la carta a meno che
non sia stata ritirata dall'ATM per qualche motivo.
Se la banca determina che il PIN del cliente e' non valido, l'ATM
richiedera' di inserire nuovamente il PIN. Dopo tre volte la carta viene
prelevata dall'ATM. Se una transazione fallisce (a parte per il PIN non
valido) l'ATM scrivera' sul display il perche' e chiedera' al cliente se
vuole eseguire un'altra transazione. L'ATM fornira' al cliente una
ricevuta stampata per ogni transazione di successo, che mostri la
data, l'ora, la locazione della macchina, il tipo di transazione, il conto o
i conti coinvolti, la somma, e finira' con la scrittura del saldo
considerando anche l'ultima operazione eseguita.
L'ATM ha un interruttore che permette ad un operatore di accendere o
spegnere la macchina. Dopo che l'operatore ha acceso la macchina
dovra' inserire a mano l'ammontare di soldi presenti nella macchina.
La macchina potra' essere spenta solamente quando non sta servendo
un cliente. La macchina viene spenta per permettere ad un operatore
di rimuovere i depositi, aggiungere carta/contanti etc.

### 2.2 Project Obectives

L'ATM dovra' fornire i seguenti servizi al cliente:
Prelievo di contanti da ogni possibile conto associato con la carta a
multipli di 20 euro. La banca deve approvare la transazione.
Deposito di contanti, in una busta, su qualunque account associato
alla carta. Il cliente deve inserire l'ammontare del deposito nella
busta, il quale sara' soggetto ad una ispezione manuale quando la
busta viene rimossa da un operatore. La banca deve approvare la
transazione prima che l'ATM accetti la busta.
Trasferimento di soldi tra due conti associati alla carta.
Verifica del Saldo su qualunque conto associato alla carta.

<a name="p3"></a>

## 3. Requirements

| Priorità | Significato             |
| -------- | ----------------------- |
| M        | **Mandatory:**          |
| D        | **Desiderable:**        |
| O        | **Optional:**           |
| E        | **future Enhancement:** |

<a name="sp3.1"></a>

### 3.1 Stakeholders

1. Cliente : Il cliente è un utente che ha uno o più conti aperti con la banca, e il suo obiettivo è quello di eseguire operazioni sui suoi conti correnti
2. Banca : E' la depositaria dei conti correnti di ogni Cliente, e vuole costruire il software per il bancomat pechè vuole via via diminuire i cassieri per abbattere i costi
3. Operatore : E' il manutentore del bancomat.

<a name="sp3.2"></a>

### 3.2 Functional Requirements

| ID  | Descrizione | Priorità |
| --- | ----------- | -------- |
| 1.0 | XXXXX       | M        |

<a name="sp3.3"></a>

### 3.2 Non-Functional Requirements

| ID  | Descrizione | Priorità |
| --- | ----------- | -------- |
| 1.0 | XXXXX       | M        |

![Diagram](imgs/atm.png)
