FROM golang:bookworm AS base

WORKDIR /build

COPY go.mod go.sum ./

RUN go mod download

COPY . .

RUN go build -o dokohabi-backend

CMD ["/build/dokohabi-backend"]
