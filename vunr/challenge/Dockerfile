FROM golang:1.26rc2

WORKDIR /app

COPY src/ .
COPY flag.txt .

RUN go mod tidy
RUN go build -o app main.go

EXPOSE 8081
CMD ["./app"]
