FROM node:18-alpine

WORKDIR /app

# Copy package files first
COPY package*.json ./
RUN if [ -f package-lock.json ]; then npm ci; else npm install; fi

# Copy the rest of the code
COPY . .

# Expose frontend port
EXPOSE 3000

# Start frontend
CMD ["npm", "run", "dev"]