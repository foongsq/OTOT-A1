FROM node:16.14.2
ENV NODE_ENV=production

WORKDIR /app

COPY package*.json .
COPY package-lock.json* .
RUN npm install --production

COPY . .

EXPOSE 3000

CMD ["node", "index.js"]
