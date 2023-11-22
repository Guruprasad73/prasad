FROM golang:latest
WORKDIR /hema1
COPY go.mod go.sum ./
RUN go mod download
COPY . .
RUN go build -o main .
EXPOSE 12345
CMD ["./main"]
