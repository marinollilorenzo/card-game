# card-game

Piccola app desktop Java Swing, realizzata come progetto scolastico delle scuole superiori. L'utente puo scegliere tra tre giochi di carte classici: Blackjack, Sette e Mezzo e Solitario. La GUI gestisce la scelta del gioco, la pesca delle carte, il punteggio e il riavvio usando immagini locali dei mazzi.

## 📑 Indice

- [Caratteristiche Principali](#-caratteristiche-principali)
- [Prerequisiti](#-prerequisiti)
- [Installazione](#-installazione)
- [Utilizzo](#-utilizzo)
- [Struttura del Progetto](#-struttura-del-progetto)
- [Configurazione (Variabili d'Ambiente)](#-configurazione-variabili-dambiente)
- [Contribuire](#-contribuire)
- [Licenza](#-licenza)

## ✨ Caratteristiche Principali

- GUI semplice in Java Swing per un progetto scolastico
- Tre giochi: Blackjack, Sette e Mezzo e Solitario
- Supporto per mazzi francesi e triestini
- Immagini delle carte caricate da cartelle locali
- Riavvio partita e visualizzazione punteggio

## 🛠 Prerequisiti

- Java JDK [versione]
- (Opzionale) Eclipse IDE per importare il progetto

## 🚀 Installazione

```bash
# 1. Clona il repository
git clone [https://github.com/tuo-utente/card-game.git](https://github.com/tuo-utente/card-game.git)

# 2. Entra nella directory
cd card-game

# 3. Compila i sorgenti
javac -d bin $(find src -name "*.java")
```

Se usi Eclipse, importa il progetto come progetto esistente (sono presenti .project e .classpath).

## 💻 Utilizzo

```bash
# Avvia la classe principale
java -cp bin it.volta.ts.marinollilorenzo.setteemezzo.boundary.Main
```

Esempio dal codice:

```java
new Console().esegui();
```

Dopo l'avvio, scegli un gioco e usa i pulsanti della GUI (Pesca, Sto, Restart).

## 📁 Struttura del Progetto

```plaintext
card-game/
├── src/                          # Sorgenti Java
│   └── it/volta/ts/...            # Package
├── bin/                          # Classi compilate (generate)
├── CARTEFRANCESI/                # Immagini mazzo francese
├── CARTETRIESTINE/               # Immagini mazzo triestino
├── .project                      # File progetto Eclipse
└── .classpath                    # Classpath Eclipse
```

## ⚙️ Configurazione (Variabili d'Ambiente)

Non sono richieste variabili d'ambiente.

Nota: il codice si aspetta cartelle `carteFrancesi` e `carteTriestine`. Su file system case-sensitive, rinomina le cartelle oppure aggiorna i percorsi in `Config.setDeckPath()`.

## 🤝 Contribuire

- Fai un fork del progetto
- Crea un branch per la feature (`git checkout -b feature/NuovaFeature`)
- Fai il commit dei cambiamenti (`git commit -m "Aggiungi NuovaFeature"`)
- Fai il push del branch (`git push origin feature/NuovaFeature`)
- Apri una Pull Request

## 📄 Licenza

Distribuito sotto la licenza [Nome Licenza, es. MIT]. Vedi il file LICENSE per maggiori informazioni.
