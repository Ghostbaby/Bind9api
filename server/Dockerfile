FROM centos:centos7
RUN yum install -y gcc python python-pip libxslt-devel python-devel python-setuptools screen mc net-tools vim ntpdate
RUN easy_install pip
ADD requirements.txt /src/pip.txt
RUN cd /src;pip install -U setuptools; pip install -r pip.txt
ADD . /src
RUN yum clean all
WORKDIR /src
