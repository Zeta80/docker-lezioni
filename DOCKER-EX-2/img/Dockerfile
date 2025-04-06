# Usa un'immagine con Node.js preinstallato
FROM node:18

# Imposta la cartella di lavoro dentro il container
WORKDIR /app

# Copia il file package.json e installa le dipendenze
COPY package.json package-lock.json ./
RUN npm install

# Copia il resto dei file
COPY ./appconf .

# Espone la porta 3000 (se il server la usa)
EXPOSE 3000

# Avvia l’applicazione
CMD ["node", "app.js"]
