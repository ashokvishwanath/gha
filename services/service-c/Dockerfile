FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy source
COPY server.js .

# Expose port and run
EXPOSE 5000
CMD ["node", "server.js"]