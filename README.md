# OpenTrials Public and Private Registries

[![Gitter](https://img.shields.io/gitter/room/opentrials/chat.svg)](https://gitter.im/opentrials/chat)
[![Issues](https://img.shields.io/badge/issue-tracker-orange.svg)](https://github.com/opentrials/opentrials/issues)
[![Docs](https://img.shields.io/badge/docs-latest-blue.svg)](http://docs.opentrials.net/en/latest/developers/)

This is [data package](http://dataprotocols.org/data-packages/) with
information on public and private registries of clinical trials.  It
intended to be used to track sources of trial data for the
[OpenTrials](http://opentrials.net) platform and to document existing
and possible methods of data extraction.

The majority of information about registries comes from the
[WHO ICTRP](http://www.who.int/ictrp/network/primary/en/)
(International Clinical Trials Registry Platform) and the websites of
the individual registries.

For registers that are members of WHO's ICTRP, another option for data
acquisition would be to write a generic parser for the XML dump
provided to ICTRP.  We would also need to source the dump URL per
register.

## Existing Tooling for Scraping Clinical Trials Data

### ClinicalTrials.gov

Many options for scraping Clinical Trials exist.  It is the largest
source for structured clinical trials data.  The scraper we will use
has been started here:

https://github.com/roll/clinicaltrials-scraper

### ISRCTN.org

This is currently a very basic scraper for scraping ISRCTN (currently
only downloading identifiers e.g. ISRCTN41598423, but can be easily
extended).

https://github.com/annapowellsmith/isrctn

### EU Clinical Trials Register (EU-CTR)

There are comparatively few options for scraping EU Clinical Trials
Register data, but a potentially useful R package for retrieving both
CT and EU data exists here.

https://github.com/rfhb/ctrdata

### Australian New Zealand Clinical Trials Registry (ANZCTR)

There is an existing scraper written for scraping data from the
Australia and New Zealand register here:

https://classic.scraperwiki.com/scrapers/australia_new_zealand_clinical_trials/

https://github.com/tfmorris/australia_new_zealand_clinical_trials/blob/master/scraper.py

### Brazilian Clinical Trials Registry (ReBec)

This is both the code and scraper for the Brazilian Clinical Trials
Registry.  The repo actually contains a very small dump (57 trials in
XML form) in the repo.  Trials have WHO's UTN
([Uniform Trial Number](http://www.who.int/ictrp/unambiguous_identification/utn/en/)):
Another option for data acquisition would be to write a generic parser
for registers that provide XML dumps to ICTRP.  DUMP_URL =
'http://www.ensaiosclinicos.gov.br/rg/all/xml/ictrp'.

https://github.com/bireme/opentrials/tree/master/data

### Japan Primary Registries Network (JPRN)

This is a scraper for the Japanese network of clinical trials.  We
would most likely create an entirely new scraper:

https://github.com/nick111/MedicalDataCrawl/commit/bdefcfa27009dca60d89edc40a806b19be2dd3a9

### Clinical Trial Registry of the University Medical Center Freiburg

No existing tooling found.  Would write new scraper.

### DeReG - German Registry for Somatic Gene-Transfer Trials

No existing tooling found.  Would write new scraper.

### Centre for Clinical Trials, University of Hong Kong

No existing tooling found.  Would write new scraper.

### Chinese Clinical Trial Registry (ChiCTR)

No existing tooling found.  Would write new scraper.

### Clinical Research Information Service (CRiS), Republic of Korea

No existing tooling found.  Would write new scraper.

### Clinical Trials Registry - India (CTRI)

No existing tooling found.  Would write new scraper.

### Cuban Public Registry of Clinical Trials(RPCEC)

No existing tooling found.  Would write new scraper.

### German Clinical Trials Register (DRKS)

No existing tooling found.  Would write new scraper.

### Iranian Registry of Clinical Trials (IRCT)

No existing tooling found.  Would write new scraper.

### Thai Clinical Trials Registry (TCTR)

No existing tooling found.  Would write new scraper.

### The Netherlands National Trial Register (NTR)

No existing tooling found.  Would write new scraper.

### Pan African Clinical Trial Registry (PACTR)

No existing tooling found.  Would write new scraper.

### Sri Lanka Clinical Trials Registry (SLCTR)

No existing tooling found.  Would write new scraper.

### UMIN CTR Website

No existing tooling found.  Would write new scraper.

### JapicCTI Website

No existing tooling found.  Would write new scraper.

### JMACCT CTR Website

No existing tooling found.  Would write new scraper.

### NIHR Clinical Research Network

No existing tooling found.  Would write new scraper.

### South African National Clinical Trials Register

No existing tooling found.  Would write new scraper.

### International Prospective Register of Systematic Reviews

No existing tooling found.  Would write new scraper.

## Other Tools

### ClinicalTrials.gov

> Using publicly available and downloadable data from
> ClinicalTrials.gov, a restructured and reformatted relational
> database was developed. This is referred to as the database for
> Aggregate Analysis of ClinicalTrials.gov (AACT).

https://www.ctti-clinicaltrials.org/what-we-do/analysis-dissemination/state-clinical-trials/aact-database

> Python classes / functions to parse Clinical Trial data in the form
> of XML returned from clinicaltrials.gov.

https://github.com/pjfan/ClinicalTrialsParser

### Trialverse

> Trialverse aims to enable world-wide collaboration on extracting
> data and meta-data on existing clinical trials, and to eventually
> reduce the duplication of effort inherent in the current systematic
> review and evidence-based decision making processes. It is part of
> ADDIS 2, a drugis.org project, and is currently in early
> development.

https://github.com/drugis/trialverse

https://trialverse.org/

### CrossRef Clinical Trials Importer

Not exactly a scraper, but tooling for importing clinical trials data.
Most useful for providing regular expressions (and tests!) for
matching different clinical trials identifiers (e.g. ISRCTN41598423,
NCT02590237, etc.):

https://github.com/CrossRef/clinical-trials-importer/blob/develop/resources/clinical-trial-registries.edn
