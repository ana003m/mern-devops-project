# Use Node.js 18 Alpine image
FROM node:18-alpine

WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install --production

# Copy the rest of the server code
COPY . .

# Expose server port
EXPOSE 5000

# Start the server
CMD ["node", "server.js"]
