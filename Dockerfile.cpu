FROM floydhub/dl-docker:cpu

# File Author / Maintainer
MAINTAINER MB

RUN apt-get update && apt-get install -y \
    curl \
    git \
    graphicsmagick \
    libssl-dev \
    libffi-dev \
    python-dev \
    python-pip \
    python-opencv \ 
    python-numpy \
    python-nose \
    python-scipy \
    python-pandas \
    python-protobuf \
    python-openssl \
    wget \
    zip \
	graphviz \
&& apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# install lmdb (fast database. depends on libffi-dev, python-dev, build-essential; requires pip for installation. lmdb python not available through apt-get.floydhub/dl-docker:cpu only installs c-version).
RUN pip install lmdb

# install pydot (again?). xx this may need changing
RUN pip install pydot
