### Gets the description (all predicates and values) of an entity and all its equivalents.
### Original SPARQL query:
##
## SELECT ?predicate ?object WHERE {
##  { dbpedia:Barack_Obama ?predicate ?object }
## UNION
##  { ?subject owl:sameAs dbpedia:Barack_Obama .
##    ?subject ?predicate ?object } }
##
### Note that owl:sameAs is not represented in the query as equivalence management
### is deferred to the compiler logic for SPARQL.
id/barack_obama