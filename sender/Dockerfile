FROM golang:1.16-alpine

WORKDIR /app

COPY go.mod ./
COPY go.sum ./
ADD https://raw.githubusercontent.com/vishnubob/wait-for-it/master/wait-for-it.sh .
RUN go mod download

COPY *.go ./

RUN go build -o /sender

CMD sleep 20 && /sender
