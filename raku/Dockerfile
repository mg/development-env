FROM arm64v8/alpine

RUN apk add rakudo zef
RUN adduser --disabled-password --gecos '' raku
USER raku
WORKDIR "/home/raku"
