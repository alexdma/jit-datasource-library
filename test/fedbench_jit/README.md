# FedBench queries for JIT data integration (ECAPI query language)

The reference language for these queries is an expanded version of the one supported by the [MK:Smart Entity-Centric API](http://github.com/mk-smart/entity-centric-api).

    {hostname}[/attribute|attribute.../value]?[attribute[/attribute]]
  
For example, a query for retrieving all the filmwork of someone either identified as, or named like `clint_eastwood` is:

    http://example.org/api/type/person/id|name/clint_eastwood?filmwork

This directory contains a collection of queries converted from those of the [FedBench](http://fedbench.fluidops.net) benchmark for federated queries.