# patient-service/Dockerfile
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install --production

# Copy source code
COPY . .

# Expose the service port
EXPOSE 5004

# Start the service
CMD ["npm", "start"]
