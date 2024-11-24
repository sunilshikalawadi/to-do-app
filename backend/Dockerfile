FROM node:14-alpine3.12

# Set the working directory
WORKDIR /app

# Copy package.json and install dependencies (if any)
COPY package.json ./
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose port 4000
EXPOSE 4000

# Start the app (make sure index.js is the correct entry point)
CMD ["node", "index.js"]
