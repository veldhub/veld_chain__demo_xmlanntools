# veld_chain_demo_xmlanntools

This repo is a demo veld chain, integrating the code veld 
https://github.com/veldhub/veld_code__xmlanntools which is a veldified version of 
https://github.com/czcorpus/xmlanntools 

The demo chains here are implementing the upstream example data and processing as explained here: 
https://github.com/czcorpus/xmlanntools/blob/main/examples/README.md

## requirements

- git
- docker (compose)

Note, depending on your docker compose version, you might need to replace `docker compose ...`
(newer) with `docker-compose` (older).


## how to reproduce

Clone this repo with all submodules:

```
git clone --recurse-submodules https://github.com/veldhub/veld_chain__demo_xmlanntools.git
```

cd into it and execute a chain veld with:
```
docker compose -f <chain yaml> up
```
e.g.
```
docker compose -f veld_simple_poetry1_step1_xml2standoff.yaml up
```

Or to run a multichain consisting of individual sub chains, e.g. the TEI example 
( https://github.com/czcorpus/xmlanntools/blob/main/examples/README.md#tei_example1 ), run :
```
docker compose -f veld_tei_example1_all_steps.yaml up
```

## more information

See inside the respective chain yaml files within this repo, or the code veld yaml files under
`./code/veld_code__xmlanntools/`, for more information on individual chain / code velds.

