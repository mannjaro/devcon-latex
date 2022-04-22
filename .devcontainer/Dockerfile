FROM paperist/texlive-ja:latest

WORKDIR /workspace

COPY ./package.json ./

COPY ./package-lock.json ./

RUN apt update && apt -y upgrade && \
    apt install -y curl gcc g++ make

RUN curl -sL https://deb.nodesource.com/setup_lts.x | bash && \
    apt install -y nodejs