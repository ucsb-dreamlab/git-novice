FROM ghcr.io/rocker-org/devcontainer/r-ver:4

# copy workbench setup script into container
COPY setup.R /tmp/setup.R

# install workbench dependencies
RUN sudo apt update && apt install -y libxslt1-dev

# install workench
RUN Rscript /tmp/setup.R