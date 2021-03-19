FROM rocker/geospatial:4.0.2

# Install additional required R libraries
COPY ./requirements.R /tmp/requirements.R
RUN Rscript /tmp/requirements.R

ENV LANG=C.UTF-8
ENV DEBIAN_FRONTEND=noninteractive

# Install all TeX and LaTeX dependences
# verify latex version
#RUN latex --version

# verify tlmgr version
#RUN tlmgr --version

# install texlive necessary packages
RUN tlmgr install \
  latex-amsmath-dev \
  iftex \
  euenc \
  fontspec \
  tipa \
  unicode-math \
  xunicode \
  kvoptions \
  ltxcmds \
  kvsetkeys \
  etoolbox \
  xcolor \
  auxhook \
  bigintcalc \
  bitset \
  etexcmds \
  gettitlestring \
  hycolor \
  hyperref \
  intcalc \
  kvdefinekeys \
  letltxmacro \
  pdfescape \
  refcount \
  rerunfilecheck \
  stringenc \
  uniquecounter \
  zapfding \
  pdftexcmds \
  infwarerr \
  fancyvrb \
  framed \
  booktabs \
  mdwtools \
  grffile \
  filehook \
  makecmds \
  polyglossia \
  natbib

# verify 
#RUN texlive-xetex --version
