### Gets the values for selected predicates of all the entities (and their
### equivalents) that match one attribute value and one property path value.
### Original SPARQL query:
##
## SELECT ?film ?director ?genre WHERE {
##   ?film dbpedia-owl:director ?director.
##   ?director dbpedia-owl:nationality dbpedia:Italy .
##   ?x owl:sameAs ?film .
##   ?x linkedMDB:genre ?genre }
##
### The conversion from dbpedia-owl:nationality to country is handled by the 
### microcompiler for the nytimes dataset. Similarly for dbpedia-owl:director
### and linkedMDB:genre
director//country/italy?director&genre