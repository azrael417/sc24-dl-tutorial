ARG DLFW_VERSION
FROM nvcr.io/nvidia/pytorch:${DLFW_VERSION}-py3

RUN pip install parameterized

ENV SCDLTUT_VERSION=0.1
RUN cd /opt && git clone -b tkurth/mp-fixes https://github.com/azrael417/sc24-dl-tutorial.git
ENV PYTHONPATH=${PYTHONPATH}:/opt/sc24-dl-tutorial

#COPY distributed/layers.py /opt/sc24-dl-tutorial/distributed/layers.py
#COPY networks/vit.py /opt/sc24-dl-tutorial/networks/vit.py
#COPY distributed/helpers.py /opt/sc24-dl-tutorial/distributed/helpers.py
