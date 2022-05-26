FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update -y && apt install -y git curl build-essential && \
    # https://www.rust-lang.org/tools/install
    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs > install.sh && \
    chmod +x ./install.sh && sh -c './install.sh -y'
WORKDIR /rust-env
#ENV PATH="~/.cargo/bin:$PATH"

CMD [ "bash" ]