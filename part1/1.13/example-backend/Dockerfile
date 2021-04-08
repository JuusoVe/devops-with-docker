FROM golang:1.16-alpine3.13

EXPOSE 8000

WORKDIR /usr/src/app

COPY . .

RUN go build

CMD PORT=8000 REQUEST_ORIGIN=http://localhost:3000 ./server

