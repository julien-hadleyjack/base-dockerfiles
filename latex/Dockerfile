FROM ubuntu:latest

ENV USER=root

RUN apt-get update && apt-get install -y \
  biber \
  make \
  pandoc \
  python3-pil \
  python3-pip \
  texlive-full \
  texlive-latex-extra \
  wget \
  xzdec

RUN pip3 --no-cache-dir install \
  docopt \
  jinja2 \
  pillow \
  pygments

RUN tlmgr init-usertree && tlmgr install \
  minted

WORKDIR /document