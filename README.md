# veld_chain_demo_xmlanntools

This repo contains [chain velds](https://zenodo.org/records/13322913) integrating the code velds 
from https://github.com/veldhub/veld_code__xmlanntools which is a veldified version of 
https://github.com/czcorpus/xmlanntools 

The demo chains here wraps the upstream example data and processing workflows as explained here: 
https://github.com/czcorpus/xmlanntools/blob/main/examples/README.md

## requirements

- git
- docker compose (note: older docker compose versions require running `docker-compose` instead of 
  `docker compose`)

Clone this repo with all its submodules
```
git clone --recurse-submodules https://github.com/veldhub/veld_chain__demo_xmlanntools.git
```

## how to reproduce

Open any respective veld yaml file for more information.

Execute one with:
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

