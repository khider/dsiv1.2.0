FROM continuumio/miniconda3
COPY . .
RUN apt-get update && apt-get install -y \
gettext-base
RUN conda env create -f environment.yml
RUN echo "source activate climate" > ~/.bashrc
ENV PATH /opt/conda/envs/climate/bin:$PATH
