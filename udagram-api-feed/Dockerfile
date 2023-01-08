FROM node:16
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied where available (npm@5+)
COPY package*.json ./
RUN npm ci 
# Bundle app source
COPY . .

# /// copie le dossier du conteneur et le met sur Docker 

EXPOSE 8080
CMD [ "npm", "run", "dev" ]




# //docker build -t udagram-api-feed .

# docker tag udagram-api-feed brice123456789/udagram-api-feed //etape importante

# docker push brice123456789/udagram-api-feed