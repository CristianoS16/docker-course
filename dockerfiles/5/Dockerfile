FROM golang AS build

ENV GO111MODULE=off

WORKDIR /app 
ADD . /app
RUN go build -o mygo

FROM alpine
WORKDIR /giropops 
COPY --from=build /app/mygo /giropops/

ENTRYPOINT ./mygo
