# FROM node:14 

# WORKDIR /app

# COPY . /app

# RUN npm install

# CMD node app.js

FROM node:14 

WORKDIR /app

# To dependency install first, COPY npm dependency before install
COPY package*.json ./

# To security, Select Exec Case
RUN ["npm", "install"]

COPY . .

# To security, Select Exec Case
CMD ["node", "app.js"]
