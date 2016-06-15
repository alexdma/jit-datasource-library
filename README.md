# Library of data sources for JIT data integration
A library of configurations, functions and templates for integrating open data sources via just-in-time operations as in the MK:Smart entity-centric API, http://github.com/mk-smart/entity-centric-api

## Contents
The first batch of Linked Open Data source configurations can be found by navigating to [configurations/ecapi/v1](configurations/ecapi/v1). Here you can find some utility functions for all data sources, as well as source-specific configurations in the subdirectories.

## Requirements
- A scripting engine that supports JavaScript (e.g. [Rhino](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/Rhino))
- A just-in-time data integration engine - currently only the [MK:Smart ECAPI](http://github.com/mk-smart/entity-centric-api) is known to contain one, which will be released as a separate library soon.

## Structure of a data source configuration
- `ecapi:microcompilers` contains microcompiler functions organised by attribute name. Each function takes a single parameter that is an object with all the attribute-value pairs of the original query
- `ecapi:query_skeletons` contains query templates organised by attribute name. Tokens of the form `<[attribute]>` are meant to be replaced with a call to the corresponding microcompiler. Tokens of the form `?[x]?` are meant to be replaced by the query engine as it assembles the skeletons into a full query and will decide the variable name to substitute.
- `ecapi:types` contains microcompilers and query skeletons that should be applied when the input query references a specific entity type. It is a shortcut for listing them for the special attribute `type` with a given value (i.e. the entity type).
- `ecapi:specs` is an array of data source specifications; for instance, it might contain a reference to a VoID description that tells the engine which SPARQl endpoint to use.
