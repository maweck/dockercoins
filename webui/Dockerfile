FROM node:lts-slim

# Needed for node 15+ see https://stackoverflow.com/a/65443098
WORKDIR /usr/app

RUN npm install express@4.17.0
RUN npm install redis@2.8.0
COPY files/ ./files/
COPY webui.js .
CMD ["node", "webui.js"]
EXPOSE 80
