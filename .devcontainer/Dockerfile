# Use the universal development container as a base
FROM mcr.microsoft.com/devcontainers/universal:2

RUN conda install -c conda-forge -c defaults matplotlib "numpy<2.0" mdanalysis mdtraj

# Install software-properties-common and Apptainer
RUN apt-get update && apt-get install -y software-properties-common \
    && add-apt-repository -y ppa:apptainer/ppa \
    && apt-get update \
    && apt-get install -y apptainer apptainer-suid