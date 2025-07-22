FROM golang:bookworm AS base

WORKDIR /build

COPY go.mod go.sum ./

RUN go mod download

COPY . .

RUN go build -o tildex-backend

CMD ["/build/tildex-backend"]
