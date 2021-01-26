FROM node
WORKDIR /app
COPY ./src/ /app/
RUN npm install
EXPOSE 3000
#CMD [ "node", "/app/index.js" ]
ENTRYPOINT npm run start
