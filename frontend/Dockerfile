FROM node:18-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Build app
RUN npm run build

EXPOSE 5173

CMD ["npm", "run", "dev"]