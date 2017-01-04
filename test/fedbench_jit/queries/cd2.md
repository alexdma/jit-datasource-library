### Gets the values for selected predicates of an entity and all its equivalents.
### Original SPARQL query:
##
## SELECT ?party ?page WHERE {
##   dbpedia:Barack_Obama dbpedia-owl:party ?party .
##   ?x nytimes:topicPage ?page .
##   ?x owl:sameAs dbpedia:Barack_Obama }
##
### The conversion from nytimes:topicPage to homepage is handled by the 
### microcompiler for the nytimes dataset. Similarly for dbpedia-owl:party
id/barack_obama?party&homepage