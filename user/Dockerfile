FROM golang:1.18-alpine

RUN mkdir /app

RUN addgroup -S rfdgroup
RUN adduser -S -D -h /app rfduser rfdgroup
RUN chown -R rfduser:rfdgroup /app

USER rfduser

COPY main.go /app

EXPOSE 8080
CMD go run /app/main.go