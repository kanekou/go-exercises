FROM golang:latest

WORKDIR /go
ADD . /go

RUN go get -u github.com/julienschmidt/httprouter \
    github.com/codegangsta/negroni \
    github.com/russross/blackfriday \
    gopkg.in/unrolled/render.v1 \
    github.com/mattn/go-sqlite3

CMD ["go", "run", "main.go"]
