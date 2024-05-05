# Use an official Node runtime as a parent image
FROM node:14


# Set the working directory
WORKDIR /usr/src/app


# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install


# Bundle app source
COPY . .


# Expose port and start application
EXPOSE 5001
CMD ["node", "server.js"]



