# Création de l'image à partir de l'image officielle de Mode 11
FROM node:11

# Création du répertoire où sera placé l'application
RUN mkdir -p /usr/src/app

# Définition de ce répertoire comme étant celui dans lequel on va éxecuter nos commandes
WORKDIR /usr/src/app

# Copie des définitions de dépendences
COPY package.json /usr/src/app

# Installation des dépendences
RUN npm install

# Copie du code pour faire tourner l'application
COPY . /usr/src/app

# Définition du port à utiliser
EXPOSE 3000

# Démarrage de l'application
CMD ["npm", "start"]