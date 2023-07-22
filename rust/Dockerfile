FROM arm64v8/alpine

RUN apk add curl musl musl-dev libgcc gcc
RUN adduser --disabled-password --gecos '' rust
USER rust
WORKDIR "/home/rust"
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
RUN source "$HOME/.cargo/env"
ENV PATH="${PATH}:/home/rust/.cargo/bin"
