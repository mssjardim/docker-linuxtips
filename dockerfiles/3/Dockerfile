FROM golang
ADD . /src
WORKDIR /src
RUN go build -o goapp
ENTRYPOINT ./goapp
