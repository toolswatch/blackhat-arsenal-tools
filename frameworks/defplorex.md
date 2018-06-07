# DefPloreX

### Description
An Elasticsearch-based toolkit that our team uses for large-scale processing, analysis and visualization of e-crime records. In particular, we've successfully been applying DefPloreX to the analysis of deface records (e.g., from web compromises); hence its name, Def(acement) eXPlorer (DefPloreX).

The full version of DefPloreX includes:

  * A thin wrapper to interact with an Elasticsearch backend (included in this release)
  * A distributed data-processing pipeline based on Celery (example included in this release)
  * An analysis component to extract information from deface web pages
  * A features extraction component to produce a compact, numerical and categorical representation of each web page
  * A statistical machine-learning component to automatically find groups of similar web pages

The input to DefPloreX is a feed of URLs describing the deface web pages,
including metadata such as the (declared) attacker name, timestamp, reason
for hacking that page, and so on. Separately, we also have a mirror of the
web pages at the time of compromise.

### Categories
* OSINT
* Frameworks

### Black Hat sessions
[![Arsenal](https://rawgit.com/toolswatch/badges/master/arsenal/usa/2017.svg)](http://www.toolswatch.org/2017/06/the-black-hat-arsenal-usa-2017-phenomenal-line-up-announced/)

### Code 
https://github.com/trendmicro/defplorex

### Lead Developer(s)
 Federico Maggi - Trend Micro https://github.com/phretor
 Marco Balduzzi - Trend Micro https://github.com/embyte
 Vincenzo Ciancaglini - Trend Micro
 Lion Gu - Trend Micro
 Ryan Flores - Trend Micro
 

### Social Media 
* [Twitter](https://twitter.com/trendlabs)
* [DefPloreX blog post](http://blog.trendmicro.com/trendlabs-security-intelligence/defplorex-machine-learning-toolkit-large-scale-ecrime-forensics/) 
