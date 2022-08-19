FROM node:16

WORKDIR /usr/src/

COPY . .

RUN npm i && npm run build && npm run prisma:migrate && npm run prisma:deploy

EXPOSE 5000

CMD ["npm", "start"]
