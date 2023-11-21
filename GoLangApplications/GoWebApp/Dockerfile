FROM golang:latest
WORKDIR /app2
COPY go.mod go.sum ./
RUN go mod download
COPY . .
RUN go build -o main .
EXPOSE 12345
CMD ["./main"]
