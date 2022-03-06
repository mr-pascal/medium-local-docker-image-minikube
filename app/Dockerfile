# Use Node.js v12
FROM node:16-alpine

WORKDIR /usr/src/app

# Copy over the whole folder content
COPY . ./

# Make a clean npm install and only install modules
# needed for production
RUN npm ci --only=production

EXPOSE 8080

# Run the web service on container startup.
CMD [ "npm", "run", "start" ]