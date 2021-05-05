FROM node:14

# Create app directory
WORKDIR /usr/src/auth

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 8082
CMD [ "node", "server.mjs" ]

# To run container:
# # docker build . -t auth
# docker run -p 8082:80 -d auth