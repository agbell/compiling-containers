FROM golang:1.14-alpine 
WORKDIR /src

build: 
    COPY . .
    RUN go build -o /dockerfile-frontend -tags "netgo static_build osusergo" ./dockerfile/cmd/dockerfile-frontend
    ENTRYPOINT ["/dockerfile-frontend"] 
    SAVE IMAGE agbell/intercal:latest