# Créez le fichier Dockerfile dans le répertoire /backend.
# Cette image sera basée sur l'image Docker node:18-alpine.
FROM node:18-alpine
ENV PORT=3000
# Copiez le fichier package.json sur l'image.
WORKDIR /usr/src/app
COPY package.json ./
# Exécutez la commande npm install.
RUN npm install
# Copiez tous les fichier sur le conteneur (attention à avoir définir le répertoire de travail à /usr/src/app).
COPY . . 
# Définissez les commandes démmarage node ./src/server.js
CMD ["node", "./src/server.js"]