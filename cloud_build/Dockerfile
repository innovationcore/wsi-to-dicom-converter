FROM ubuntu:22.04
ARG DEBIAN_FRONTEND=noninteractive

#get dep
RUN apt-get update
RUN apt-get install -y git

#build WSI convert
WORKDIR /opt
RUN git clone https://github.com/innovationcore/wsi-to-dicom-converter
WORKDIR /opt/wsi-to-dicom-converter
RUN git checkout origin/isyntax-support
RUN opt/wsi-to-dicom-converter/cloud_build/debianBuild_isyntax.sh
