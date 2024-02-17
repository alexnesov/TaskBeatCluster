# Use Node.js version 14 as base image
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json files to the container
COPY public ./public
COPY src ./src
COPY package.json .
COPY package-lock.json .

# Install dependencies
RUN npm install

# Build the React app
RUN npm run build

# Expose port 3000 to the outside world
EXPOSE 3000

# Command to run the React app
CMD ["npm", "start"]
