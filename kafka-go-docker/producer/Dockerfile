FROM abhirockzz/kafka_go_client
WORKDIR /go/src/app
COPY ../go.mod /go/src/app/
COPY ../go.sum /go/src/app/
RUN go mod download
COPY kafka-producer.go /go/src/app/
RUN go build -o /producer
CMD ["./producer"]