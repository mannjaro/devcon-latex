FROM paperist/texlive-ja:latest

WORKDIR /workspace

RUN apt update && apt -y upgrade && \
    apt install -y curl gcc g++ make texlive-extra-utils && \
    apt-get clean && \
    apt-get autoremove -y && \
    rm -rf /var/lib/apt/lists/*

RUN curl -sL https://deb.nodesource.com/setup_lts.x | bash && \
    apt install -y nodejs && \
    apt-get clean && \
    apt-get autoremove -y && \
    rm -rf /var/lib/apt/lists/*

## Add other packages
# RUN tlmgr update --self && \
#     tlmgr install \
#         collection-bibtexextra \
#         collection-fontsrecommended \
#         collection-langenglish \
#         collection-langjapanese \
#         collection-latexextra \
#         collection-latexrecommended \
