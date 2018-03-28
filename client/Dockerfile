FROM centos:centos7
RUN yum install -y bind-utils 
COPY ddns-client /usr/local/bin/ddns-route53
ENTRYPOINT ["/usr/local/bin/ddns-route53"]
