# Use an official Node runtime as a parent image
FROM node:14


# Set the working directory
WORKDIR /usr/src/app


# Install dependencies
COPY package*.json ./
RUN npm install


# Bundle app source
COPY . .


# Build the React app
RUN npm run build



# Install serve to serve the build folder on port 3000
RUN npm install -g serve
CMD ["serve", "-s", "build", "-l", "3000"]


# Expose port
EXPOSE 3000