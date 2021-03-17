FROM rocker/geospatial:4.0.2

# Install additional required R libraries
COPY ./requirements.R /tmp/requirements.R
RUN Rscript /tmp/requirements.R

