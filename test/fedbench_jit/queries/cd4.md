### Gets the values for a property and a property path of all the entities 
### that match one attribute value, and all their equivalents.
### Original SPARQL query:
##
## SELECT ?actor ?news WHERE {
##   ?film purl:title 'Tarzan' .
##   ?film linkedMDB:actor ?actor .
##   ?actor owl:sameAs ?x.
##   ?y owl:sameAs ?x .
##   ?y nytimes:topicPage ?news }
##
### The conversion from nytimes:topicPage to webpage is handled by the 
### microcompiler for the nytimes dataset. Similarly for linkedMDB:actor
name/tarzan?actor&actor/webpage