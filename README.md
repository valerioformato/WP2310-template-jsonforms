# CAESAR + JSON Forms

## Setup

- Clonare questo repo
  `git clone https://github.com/valerioformato/WP2310-template-jsonforms.git`
- Startare un docker container con la corretta versione di NodeJS
  `docker run -it -p 3000:3000 --mount type=bind,source=$PWD/WP2310-template-jsonforms,target=/app node:14.18 /bin/bash` - All'interno del container eseguire
  `npm ci && npm start`
  n.b: La prima volta puo' richiedere decine di minuti.
- Aprire un browser e puntarlo a `http://localhost:3000`. Dovreste vedere la pagina di esempio.

## Using VSCode
Il repo contiene gia' la configurazione per poter aprire il progetto in [Visual Studio Code](https://code.visualstudio.com) tramite l'estensione "Dev Container".

## Working on it

I file piu' importanti su cui lavorare (all'inizio) sono

- `src/schema.json`: Questo file definisce lo schema del datamodel. Quali sono i campi previsti e di che tipo, che finiranno poi nell'output finale.
- `src/uischema.json`: Questo file definisce quali elementi UI creare nel form, come disporli, e a quali campi del datamodel definito nello `schema.json` sono legati.

## Based on: JSON Forms React seed App

This seed demonstrates how to use [JSON Forms](https://jsonforms.io) with React in order to render a simple form for displaying a task entity.
