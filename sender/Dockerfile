FROM golang:1.17.5-alpine

WORKDIR /app

COPY go.mod ./
COPY go.sum ./

RUN go mod download

COPY *.go ./

RUN go build -o /sender

CMD sleep 20 && /sender