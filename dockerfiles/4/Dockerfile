FROM golang

ENV GO111MODULE=off

WORKDIR /app 
ADD . /app
RUN go build -o mygo

ENTRYPOINT ./mygo
