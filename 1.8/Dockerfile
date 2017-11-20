FROM golang:1.8-alpine
RUN apk --update add git openssh
RUN go-wrapper download -u github.com/golang/dep/cmd/dep \
    && go-wrapper install github.com/golang/dep/cmd/dep \
    && rm -rf /usr/lib/go /go/src /go/pkg /var/cache/*
