FROM golang:1.18-alpine

RUN mkdir /app/
COPY main.go /app/

ENTRYPOINT ["go", "run"]

EXPOSE 8080

CMD ["/app/main.go"]