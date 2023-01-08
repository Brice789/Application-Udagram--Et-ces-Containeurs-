FROM node:16
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied where available (npm@5+)
COPY package*.json ./
RUN npm ci 
# Bundle app source
COPY . .
EXPOSE 8080
CMD [ "npm", "run", "dev" ]



# docker build -t udagram-api-user .




# docker tag udagram-api-user brice123456789/udagram-api-user //etape importante



# docker push brice123456789/udagram-api-user