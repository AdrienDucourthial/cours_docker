FROM node:20
WORKDIR /app
COPY back/package*.json ./
RUN npm install
COPY back/ .
EXPOSE 4000
CMD ["npm", "start"]