# id-dnssec-alg-nego
DNSSEC Algorithm Negotiation protocol spec

This document specifies a DNS extension that allows a DNS client to
specify a list of DNSSEC algorithms, in preference order, that the
client supports. A DNS server upon receipt of this extension can
choose to selectively respond with DNSSEC signatures using the
preferred algorithm. This mechanism may make it easier for DNS zone
operators to support signing zone data simultaneously with multiple
DNSSEC algorithms, without significantly increasing the size of DNS
responses. It will also allow an easier way to transition to new
algorithms while still retaining support for older DNS validators that
do not yet support the new algorithms.

