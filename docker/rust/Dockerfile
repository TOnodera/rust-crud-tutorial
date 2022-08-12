FROM rust:latest

RUN useradd -m -u 1000 rust -s /bin/bash
RUN rustup component add rustfmt
RUN cargo install cargo-watch
RUN cargo install diesel_cli --no-default-features --features postgres
RUN chown -R rust:rust /usr/local/cargo
USER rust