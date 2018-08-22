FROM golang AS buildando
ADD . /src
WORKDIR /src
RUN go build -o goapp

FROM alpine
WORKDIR /app
COPY --from=buildando /src/goapp /app
ENTRYPOINT ./goapp
