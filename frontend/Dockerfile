# Use official Node.js image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install frontend dependencies
RUN npm install

# Copy frontend source code
COPY . .

# Expose Vite dev server port
EXPOSE 5173

# Start React app
CMD ["npm", "run", "dev"]
