brakeman_risk_io is a small script which will use [brakeman](http://brakemanscanner.org/) to scan a Rails application for vulnerabilities and send the results to [Risk I/O](https://www.risk.io/), converting [brakeman warning types](http://brakemanscanner.org/docs/warning_types/) to the correct [WASC ID](http://projects.webappsec.org/w/page/13246975/Threat-Classification-Taxonomy-Cross-Reference-View) where possible.

Installation
------------
```
git clone git@github.com:joeyschoblaska/brakeman-risk-io.git
chmod +x brakeman-risk-io/brakeman_risk_io
```

Dependencies
------------
This script depends on the following gems:
```
brakeman
httparty
```

Usage
-----
```
RISK_IO_API_KEY=yourapikeyhere ./brakeman_risk_io ~/path/to/rails/app
```
