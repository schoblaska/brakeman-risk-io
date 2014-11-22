brakeman_risk_io is a small script which will use brakeman to scan a Rails application for vulnerabilities and send the results to Risk I/O, converting brakeman warning types to the correct WASC ID where possible.

== Installation

```
git clone git@github.com:joeyschoblaska/brakeman-risk-io.git
chmod +x brakeman-risk-io/brakeman_risk_io
```

=== Usage
```
RISK_IO_API_KEY=yourapikeyhere ./brakeman_risk_io ~/path/to/rails/app
```
