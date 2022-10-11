FROM mjgargani/puppeteer:trybe1.0

WORKDIR /app

ADD ["node_modules.tar.gz", "./"]

COPY ./e2e ./e2e

COPY ["package.json", "package-lock.json", "./"]

COPY jest.config.js .

CMD ["npm", "test"]