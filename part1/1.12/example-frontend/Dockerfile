FROM node:14.16.1-alpine3.13

EXPOSE 5000

WORKDIR /usr/src/app

COPY . .

RUN npm install

RUN REACT_APP_BACKEND_URL=http://localhost:3001/ npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]

