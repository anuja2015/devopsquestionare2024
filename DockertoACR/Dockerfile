# Stage 1: Build Stage
FROM node:23 AS build

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY samplenodejs/package*.json ./

# Install dependencies
RUN npm install --legacy-peer-deps

# Copy the application code into the container
COPY samplenodejs/ ./

# Build the application
RUN npm run build

# Stage 2: Production Stage
FROM node:23-slim

# Set the working directory in the container
WORKDIR /app

# Copy only the necessary files from the build stage
COPY --from=build /app .
COPY --from=build /app/package*.json ./

# Install only production dependencies
RUN npm install --legacy-peer-deps --only=production

# Expose the port that the application runs on
EXPOSE 3000
