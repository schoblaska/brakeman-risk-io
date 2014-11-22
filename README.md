brakeman_risk_io is a small script which uses [brakeman](http://brakemanscanner.org/) to scan a Rails application for vulnerabilities and sends the results to [Risk I/O](https://www.risk.io/), converting [brakeman warning types](http://brakemanscanner.org/docs/warning_types/) to the correct [WASC ID](http://projects.webappsec.org/w/page/13246975/Threat-Classification-Taxonomy-Cross-Reference-View) where possible.

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

Continuous Integration
----------------------
If you find this script useful, you'll probably want to run it as part of your continuous integration suite. This way, any vulnerabilities introduced to your code will be automatically discovered and posted to your Risk I/O dashboard. Most CI servers support running an arbitrary script like this one as part of your build - just make sure that brakeman and httparty are available.
