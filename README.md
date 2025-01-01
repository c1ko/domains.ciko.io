# domains.ciko.io

Documentation and Issues for the domain search engine [domains.ciko.io](http://domains.ciko.io). This repository does not contain source code.

## About the website
[domains.ciko.io](http://domains.ciko.io) enables you to to find registered domain names that reassemble a given keyword. The results are useful to find phishing domains or shadow infrastructure. Instead of only scanning for the keyword, this website also scans for deviations (also called squatting domains) that are similar to the given keyword.

## Quickstart
1. Enter a keyword in the search field on the [domains.ciko.io](http://domains.ciko.io). The keyword may only contain ASCII letters, numbers, and dashes. Enter an access token to validate the search. Press the find button.
1. The system generates a list of domains to scan, and then scans them. This may take up to 20 minutes, depending on the keyword and scan configuration. You may periodically reload the page to see newly found domains.
1. You can click on any search result to get an overview of its DNS records and subdomains.

## Engines
domains.ciko.io uses 3 engines to find squatting domains: Active DNS probing, scans of certificate transparency logs, and scans in TI datafeeds. All three engines are enabled by default. You can disable and configure the scan settings on the main page before starting the scan.
