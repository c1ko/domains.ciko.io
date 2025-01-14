# domains.ciko.io

Documentation and Issues for the domain search engine [domains.ciko.io](http://domains.ciko.io). This repository does not contain source code.

## About the tool
[domains.ciko.io](http://domains.ciko.io) enables you to to find registered domain names that reassemble a given keyword. The results are useful to find phishing domains or shadow infrastructure. Instead of only scanning for the keyword, the tool also scans for deviations (also called squatting domains) that are similar to the given keyword.

## Quickstart
1. Enter a keyword in the search field on the [domains.ciko.io](http://domains.ciko.io). The keyword may only contain ASCII letters, numbers, and dashes. Enter an access token to validate the search. Press the find button.
1. The tool generates a list of domains to scan, and then scans them. This may take up to 20 minutes, depending on the keyword and scan configuration. You may periodically reload the page to see newly found domains.
1. You can click on any search result to get an overview of its DNS records and subdomains.

### Access Token
The tool is publicly usable but requires an access token that are consumed per scan. [ciko](https://github.com/c1ko) distributes access token on various channels. If you need some access token out of sequence, please mail me at domains@ciko.io. 

I issue access token to rate limit the usage of the tool and limit waiting times. DNS scanning and enriching are network-heavy and longer lasting tasks. I provide for the entire infrastructure out of private funds, so it cannot be scaled like a commercial product.

## Engines
domains.ciko.io uses 3 engines to find squatting domains: Active DNS probing, scans of certificate transparency logs, and scans in TI datafeeds. All three engines are enabled by default. You can disable and configure the scan settings on the main page before starting the scan.

## Limitations
The tool is currently limited to 10,000 found domains and 100,000 DNS scans per keyword to limit network usage. 

## Issues / Contact
You may submit issues and requests via GitHub issues. You can also use domains@ciko.io for that purpose.

## Acknowledgements

- This tool uses the permutation engine of [dnstwist](https://github.com/elceef/dnstwist).
- Certificates for scanning are collected with [certstream](https://github.com/CaliDog/certstream-server).
