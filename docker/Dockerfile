FROM golang:1-alpine
LABEL maintainer="Amos Burton <the.amos.burton@protonmail.com>"

RUN apk add --no-cache git \
  && go get -d -v github.com/amosburton/hulk \
  && go install github.com/amosburton/hulk \
  && rm -rf ~/go/src/github.com/amosburton/hulk

ENTRYPOINT ["hulk"]

CMD ["--help"]
