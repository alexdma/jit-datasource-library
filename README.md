# Library of data sources for JIT data integration
A library of configurations, functions and templates for integrating open data sources via just-in-time operations as in the MK:Smart entity-centric API, http://github.com/mk-smart/entity-centric-api

## Contents
The first batch of Linked Open Data source configurations can be found by navigating to [configurations/ecapi/v1](configurations/ecapi/v1). Here you can find some utility functions for all data sources, as well as source-specific configurations in the subdirectories.

## Requirements
- A scripting engine that supports JavaScript (e.g. [Rhino](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/Rhino))
- A just-in-time data integration engine - currently only the [MK:Smart ECAPI](http://github.com/mk-smart/entity-centric-api) is known to contain one, which will be released as a separate library soon.
