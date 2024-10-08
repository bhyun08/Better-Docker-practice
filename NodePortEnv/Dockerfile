FROM node:14

WORKDIR /app

COPY package.json ./

RUN npm install

COPY . .

# explicit statement
EXPOSE $PROT 

CMD ["npm", "start"]

# docker run -d -p 3000:3000 --env-file ./.env