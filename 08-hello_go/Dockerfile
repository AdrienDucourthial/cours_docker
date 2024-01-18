FROM golang:1.19
WORKDIR /app
COPY . .
RUN go mod init main
RUN go mod tidy
RUN go build
EXPOSE 8080
CMD ["./main"]