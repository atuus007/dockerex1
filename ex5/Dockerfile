FROM fedora:30

COPY dance.pl /usr/src/dance.pl
RUN yum install -y perl perl-Dancer2
ENTRYPOINT ["/usr/bin/perl"]

CMD ["/usr/src/dance.pl"]
