FROM node:20-alpine

WORKDIR /app

# Cài prisma
RUN npm install -g prisma

COPY package*.json ./
RUN npm install

COPY . .

RUN prisma generate

EXPOSE 8000

CMD ["npm", "start"]
