Secret Code Game 🧠

Una riproduzione moderna e interattiva del classico gioco da tavolo Mastermind, realizzata utilizzando JavaScript puro (Vanilla JS) con architettura a moduli (ES Modules).

🎮 Obiettivo del Gioco

Il computer genera un codice segreto composto da 4 colori. Il tuo obiettivo è indovinare la sequenza esatta entro 10 tentativi.

I Colori Disponibili

🟠 Arancione | 🟡 Giallo | 🔴 Rosso | 🟢 Verde | 🔵 Blu | 🟤 Marrone

📜 Regole e Feedback

Dopo aver riempito una riga e premuto "Verifica Codice", riceverai degli indizi (pioli piccoli a destra):

⚫ Piolo Nero: Un colore è giusto e si trova nella posizione corretta.

⚪ Piolo Bianco: Un colore è presente nel codice segreto, ma si trova nella posizione sbagliata.

Nessun Piolo: Il colore non è presente nel codice segreto (o ne hai messi troppi rispetto a quanti ce ne sono nel segreto).

Esempio: Se il codice è [Rosso, Blu, Verde, Giallo] e tu provi [Rosso, Verde, Marrone, Blu], otterrai 1 Nero (per il Rosso) e 2 Bianchi (per Verde e Blu).

🚀 Come Avviare il Progetto

Poiché il progetto utilizza i Moduli ES6 (import/export), è necessario un server locale per avviarlo (non basta aprire il file HTML).

Prerequisiti

Node.js installato sul computer.

Passaggi

Clona questa repository o scarica la cartella.

Apri il terminale nella cartella del progetto.

Avvia il server locale con il comando:

npm start


Apri il browser all'indirizzo indicato (solitamente http://localhost:3000).

(Nota: Il comando usa npx serve configurato nel package.json).

🛠️ Tecnologie Utilizzate

HTML5: Struttura semantica.

CSS3: Design responsive, Flexbox e Grid per il layout.

JavaScript (ES6+): Logica modulare divisa in:

main.js: Controller principale.

game-logic.js: Algoritmo di calcolo dei pioli neri/bianchi.

ui-renderer.js: Gestione del DOM e delle animazioni.

constants.js: Configurazione centralizzata.

📂 Struttura dei File

SecretCode/
├── src/
│   ├── constants.js    # Colori e configurazioni
│   ├── game-logic.js   # Logica pura (No DOM)
│   └── ui-renderer.js  # Gestione interfaccia grafica
├── index.html          # Entry point HTML
├── main.js             # Entry point JavaScript
├── package.json        # Configurazione npm
└── README.md           # Documentazione


👨‍💻 Autore

Sviluppato da Grax
