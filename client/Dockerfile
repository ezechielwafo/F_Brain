FROM node:lts-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
CMD ["npm","run","dev"]
EXPOSE 5173
EXPOSE 4173
