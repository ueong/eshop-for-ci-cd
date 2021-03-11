FROM node:lts-alpine as build-stage
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY . .
 
EXPOSE 8094
CMD ["node", "index.js"]
