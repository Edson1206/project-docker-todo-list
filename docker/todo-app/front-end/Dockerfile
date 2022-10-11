FROM node:14-alpine

WORKDIR /app

EXPOSE 3000

COPY ["package.json", "package-lock.json", "./"]
RUN npm install

COPY ["src", "./src"] 
ADD ["node_modules.tar.gz", "./"]

CMD [ "npm", "start" ]