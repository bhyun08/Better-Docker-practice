FROM golang:1.23.1-alpine AS build

WORKDIR /app

COPY go.mod .
COPY go.sum .

RUN go mod download

COPY . .

RUN go build -o server .

FROM alpine

WORKDIR /app

COPY --from=build /app/server .
EXPOSE 8000

CMD ["./server"]