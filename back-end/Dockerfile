FROM node:16

WORKDIR /usr/src/

COPY . .

RUN npm i
RUN npm run build
RUN npm run prisma:deploy
RUN npm run prisma:seed

EXPOSE 5000

CMD ["npm", "start"]
