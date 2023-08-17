FROM golang:1.20-alpine
WORKDIR /app

COPY . .

RUN go get ./ && go build && go mod download

EXPOSE 5000
CMD ["go", "run", "main.go"]
