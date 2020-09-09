FROM golang:alpine as builder

LABEL maintainer="Amaury Euzebio amaury@a1tecnologia.info"

WORKDIR $GOPATH/src/app

COPY src/greeting/ .

RUN CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o /go/bin/app .

FROM scratch

COPY --from=builder /go/bin/app /go/bin/app

ENTRYPOINT ["/go/bin/app"]

EXPOSE 8000