FROM ubuntu:22.04
ARG DEBIAN_FRONTEND=noninteractive

#get WSI convert
WORKDIR /opt
RUN git checkout https://github.com/innovationcore/wsi-to-dicom-converter
WORKDIR /opt/wsi-to-dicom-converter
RUN opt/wsi-to-dicom-converter/cloud_build/debianBuild_isyntax.sh
